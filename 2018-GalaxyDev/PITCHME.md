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
![scale-60](assets/images/galaxy/toolshed_install.png)
</div>


---

### Github

<div class="block">
<div class="left">

Continuous integration
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


