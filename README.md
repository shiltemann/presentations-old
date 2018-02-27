# Slides

Collection of my slides and presentations

Slides available with [GitPitch](https://gitpitch.com/) under url: 

`https://gitpitch.com/shiltemann/presentations/slides?p=<subfolder name>`


## Links to Presentations

[Metagenomics using Galaxy](https://gitpitch.com/shiltemann/presentations/slides?p=2018-GalaxyEU) @ GalaxyEU conference

## Presenting slides

- `F` for Full screen
- `S` for Speaker Notes

## Developing slides

Slides must be in a file named `PITCHME.md`  
Slides automatically available at url in following form: 

`https://gitpitch.com/$user/$repo/$branch?p=$subdirectory`

Some useful links:

[Asset Sharing](https://github.com/gitpitch/gitpitch/wiki/Asset-Sharing)  
[Modular Markdown](https://github.com/gitpitch/gitpitch/wiki/Modular-Markdown)
[Offline Slideshow](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Offline)



### Offline preview

```bash
$ cd <path to presentation directory>
$ python3 -m http.server
```

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


