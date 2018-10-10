# Slides

Collection of my slides and presentations

Slides available with [GitPitch](https://gitpitch.com/) under url:

`https://gitpitch.com/shiltemann/presentations/slides?p=<subfolder name>`

or via the main slide set, which contains links to all other presentations: [https://gitpitch.com/shiltemann/presentations/slides](https://gitpitch.com/shiltemann/presentations/slides)

## Links to Presentations

| Title                                                                                                   | Where                                | When             |
|---------------------------------------------------------------------------------------------------------|--------------------------------------|------------------|
|[Microbiota Analysis using Galaxy](https://gitpitch.com/shiltemann/presentations/slides?p=2018-GalaxyEU) | Galaxy User Conference, Freiburg     | March 15-16 2018 |
|[My life as a bioinformatician](https://gitpitch.com/shiltemann/presentations/slides?p=2018-LIACS) | LIAXX Informatics Ladies Day, LIACS Leiden | May 18 2018      |
|[Data Analysis in Galaxy](https://gitpitch.com/shiltemann/presentations/slides?p=2018-StreeklabHaarlem)  | Streeklab Haarlem                    | July 5 2018      |
|[Galaxy Tool Devlopment](https://gitpitch.com/shiltemann/presentations/slides?p=2018-GalaxyDev)          | EMC Rotterdam                        | 9 July 2018      |
|[Galaxy Training Network](https://gitpitch.com/shiltemann/presentations/slides?p=2018-ECCB)              | ECCB, Athens Greece                  | 10 September 2018|
|[Galaxy for Diagnostics](https://gitpitch.com/shiltemann/presentations/slides?p=2018-SURF)              | SURF Life Science Seminar            | 12 October 2018  |


## Presenting slides

- `F` for Full screen
- `S` for Speaker Notes

## Developing slides

Slides must be in a file named `PITCHME.md`
Slides automatically available at url in following form:

`https://gitpitch.com/$user/$repo/$branch?p=$subdirectory`

Some useful links:

- [Asset Sharing](https://github.com/gitpitch/gitpitch/wiki/Asset-Sharing)
- [Modular Markdown](https://github.com/gitpitch/gitpitch/wiki/Modular-Markdown)
- [Offline Slideshow](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Offline)



### Offline development

Using docker (gitpitch + gitlab), full instructions [here](docker/)

```bash
$ cd docker
$ docker-compose up
```

Use inotify to push changes to local gitpitch on every modification of slide.

From the slides folder do:

```
while inotifywait -r --exclude ".*.swp" -e modify . ; do git reset HEAD~ && git add PITCHME.md PITCHME.yaml ../assets/images/*  && git commit -m "add content" && git push -f gitpitch; done
```

- Be sure not to save again until the update and push has completed
- This will overwrite your last commit to keep history clean, use with care!!


### Set background image for a slide

```md
---?image=assets/image/lukas_blazek.jpg
```

### Code Snippets and Syntax Highlighting

```markdown
---?code=path/to/code.py&lang=python&title=Python File
```

### Include markdown file

NOTE: this only works for the top-level `PITCHME.md` file

```markdown
---?include=md/intro.md
```


