# Galaxy Tool Development


+++

### Overview

- Galaxy Ecosystem
- Galaxy Tool Development with Planemo
- Conda Packaging?
- Galaxy Flavours (docker)

---

### Galaxy Ecosystem

![](assets/images/galaxy/galaxy_ecosystem.png)

Note:
- Conda for dependencies
  - get mulled container for free
  - biocontainers
- Planemo for wrapper development
- Training materials

---

### Galaxy Tool Shed

The Galaxy App store

![](assets/images/galaxy/toolshed_screenshot.png)


---

### Galaxy Tool Shed

<div>
![scale-60](assets/images/galaxy/galaxy_admin_toolsheds.png)
</div>
<div>
![scale-50](assets/images/galaxy/toolshed_install.png)
</div>

---

### IUC

Intergalactic Utilities Commission

![scale-60](assets/images/galaxy/iuc.png)

<div class="small">
Tool repo: https://github.com/galaxyproject/tools-iuc <br>
Best practices: http://galaxy-iuc-standards.readthedocs.io/en/latest/best_practices.html
</div>

---

### Github

<div class="block">
<div class="left">

Travis Continuous Integration
<br>
<ul>
<li>Linting xml wrappers</li>
<li>Flake8 testing</li>
<li>Functional tests</li>
<li>Tool shed upload</li>
</ul>
</div>

<div class="right">
![](assets/images/galaxy/travis_tool_testing.png)
</div>
</div>

<div class="bottom small">
IUC: https://github.com/galaxyproject/tools-iuc
<br>
EMC: https://github.com/erasmusmc-bioinformatics/galaxytools-emc
</div>

---

![](assets/images/galaxy/planemo_logo.png)

Galaxy tool development framework
- Lint your tool xml wrapper
- Run functional tests
- Planemo serve (deploy tools locally)
- Upload to Tool Shed
- ...

<br>
<div class="bottom">
Documentation: https://planemo.readthedocs.io
</div>
---

### Training

![scale-60](assets/images/galaxy/training_materials_website.png)

https://training.galaxyproject.org

---

### Today

<div class="leftalign">
<ul>
<li>Morning:</li>
 <ul>
  <li>Intro to tool wrapping </li>
  <li> Hands-on tool wrapping: seqtk </li>
 </ul>
<li>Optional:</li>
 <ul>
  <li> Conda </li>
  <li> Docker Galaxy Flavours </li>
  <li> .. suggestions? requests? </li>
 </ul>
<li>Afternoon:</li>
 <ul>
  <li> Wrap your own! </li>
  <li> https://github.com/ErasmusMC-Bioinformatics/galaxytools-emc/issues/51 </li>
 </ul>
</ul>
</div>

---

### Useful links

- [Training Materials](https://training.galaxyproject.org)
- [Tool Schema Definition](https://docs.galaxyproject.org/en/latest/dev/schema.html)
- [Planemo Documentation](https://planemo.readthedocs.io/en/latest/)
- [IUC Best Practices](http://galaxy-iuc-standards.readthedocs.io/en/latest/best_practices.html)
- Tool repoitories: [IUC](https://github.com/galaxyproject/tools-iuc) and [EMC](https://github.com/ErasmusMC-Bioinformatics/galaxytools-emc)
- [Tool Shed](https://toolshed.g2.bx.psu.edu/) and [Test Tool Shed](https://testtoolshed.g2.bx.psu.edu/)
- [Bioconda recipes](https://github.com/bioconda/bioconda-recipes)
- [Saskia's Galaxy Tool Cheat Sheet](https://github.com/shiltemann/cheatsheets/blob/master/galaxy-tools.md)

<br><br>
<div class="bottom small">These slides: https://gitpitch.com/shiltemann/presentations/slides?p=2018-GalaxyDev</div>


