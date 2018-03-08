---?image=2018-GalaxyEU/images/background.jpg

<div class="white">
<h2 class="white"> Microbiota Analysis using Galaxy </h2>

Saskia Hiltemann 

</div>

---
 
### Overview

- Background
- Analysis pipeline
- Clinical Results

---

### Microbiota

![Video](https://www.youtube.com/embed/htbeJhtFAXw)

---

### A Brief History

<div class="left small center">

<ul>
  <li> Antonie van Leeuwenhoek is commonly known as the *Father of Microbiology* </li>

![scale-30](2018-GalaxyEU/images/leeuwenhoek.jpg)

  <li> In 1676, he discovered **animalcules** when he turned his microscope to a drop of rain water </li>
</ul>

</div>

<div class="right">

<!-- ![scale-70](2018-GalaxyEU/images/animalcules.gif) -->
![](2018-GalaxyEU/images/leeuwenhoek-microscope-animalcules.jpg) 

</div>

Note:
Antonie van Leeuwenhoek was Dutch scientist, best known for his work in microscopy 

In 1676 he turned his microscope at a drop of rain water and was surprised to find 
what looked like tiny animals, which he called **animalcules** 


---

Pasteur: Food spoilage
von Koch: Germ theory

---

### Why study the microbiome?


<div class="block">
<div class="left small middle">
<br><br> 
<ul>
  <li> > 10 times more cells than you </li>
  <li> > 100 times more genes than you </li>
  <li> > 1000 different species </li>
</ul>
</div>
<div class="right">

![](2018-GalaxyEU/images/human_microbiome.png)

</div>
</div>

Sometimes referred to as your *second genome* 

---


### Dysbiosis

- Microbial imbalance in the body
- Linked to a large number of disease phenotypes
  - Obesity, Diabetes
  - Asthma, Allergies
  - Crohn's disease, Ulcerative colitis
  - Cancer, IBS, Autism

![scale-40](2018-GalaxyEU/images/microbiota-disease.jpg)

---

monocultures

---

### Approaches

- Amplicon sequencing 
- Shotgun sequencing 

---

### Shotgun Sequencing

<div class="left">
<ul>
<li> Sequence everything </li>
<li> Expensive </li>
<li> More information </li>
<li> Higher complexity </li>
</ul>
</div>

<div class="right">
![](2018-GalaxyEU/images/shotgun-puzzles.png)
</div>

---

### Amplicon Sequencing

- Targetted approach (e.g. 16S/18S rRNA gene)
- Amplifies bacteria, not host or environmental fungi, plants

![scale-50](2018-GalaxyEU/images/16S_gene.png)

--- 

### 16S rRNA gene

- Highly conserved regions 
  - easy to target across all bacteria
- Variable regions 
  - distinguish between different types of bacteria

![scale-70](2018-GalaxyEU/images/16S_variableregions.jpg)

Note:
around 1500 nucleotides long

---


### Streeklab Haarlem

Hospitals and clinics send their samples (stool/urine/nasal)
for analysis

- determine microbiota present
- determine antibiotics to use

---

### Streeklab Haarlem

current method: cultures

pilot: 16S rRNA sequencing


---

### Experiment Design

Micelle

3 replicates
background control

Illumina MiSeq

---


![](2018-GalaxyEU/images/so_much_data.png)

---

### Pipeline

![](2018-GalaxyEU/images/workflow.png)

---

### Pipeline

![](2018-GalaxyEU/analysis_pipeline.png)

---

### Tools

Mothur Qiime

---

### Chimera removal


- Greek mythology: hybrid animals
- Sequencing data: hybrid sequences created during PCR

<div class="left">
![scale-50](2018-GalaxyEU/images/chimera-animal.jpg)
</div>

<div class="right">
![border](2018-GalaxyEU/images/chimeras.png)
</div>

---

### OTU Clustering

**OTU**: Operational Taxonomic Unit

<div class="left">
![](2018-GalaxyEU/images/otu.png)
</div>
<div class="right">
![](2018-GalaxyEU/images/otu-clusters.png)
</div>

---

### OTU Clustering

3 main ways to do OTU picking:
  - De novo
  - Closed reference
  - Open reference


Note:
Also referred to as "OTU picking"


---

### Rarefaction

QC: Have I captured the full diversity of my sample?

![](2018-GalaxyEU/images/rarefaction.gif)


---

### Alpha Diversity


---

### Beta Diversity


---

### 

mothur, Qiime, picrust

Phinch, krona, venn, heatmaps


---

streeklab haarlem

 
