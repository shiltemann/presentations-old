# Docker Compose GitPitch with GitLab

For offline development of GitPitch presentations.

## Starting

Start docker images:

```
docker compose up
```

View presentations:

```
http://localhost:9000/<username>/<repo>/<branch>[?p=<presentation>]
```

For example: `http://localhost:9000/shiltemann/presentations/slides?p=2018-GalaxyEU`


## First time config

Open up GitLab (http://localhost:8081) and register an account with same username as
on GitHub. Then create a repository with same name as the one you are testing has on GitHub

Add the the local Gitlab as a remote for the repo:

```
$ git remote add gitpitch http://localhost:8081/shiltemann/presentations.git
```

## Preview changes

```
$ git commit <your changes>
$ git push gitpitch
```

## Troubleshooting 

If the background images are not showing, you may need to:

add the following to `/etc/nginx/sites-enabled/default`:

```
server {
  listen       80;
  server_name  gitlab;
  location / {
    proxy_pass http://127.0.0.1:8081;
} 
```
 
add to `/etc/hosts` file:

```
127.0.0.1   gitlab
```

```bash
$ sudo service network-manager restart
```
