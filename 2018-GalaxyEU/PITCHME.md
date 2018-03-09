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

Sometimes referred to as your **second genome**

---


### Dysbiosis

<div class="left small leftalign">

<ul>
<li> Microbial imbalance in the body </li><br>

<li> Causes </li>
 <ul>
  <li> Infection  </li>
  <li> Lifestyle (diet, stress) </li>
  <li> Host genetics </li>
  <li> Medications </li>
  <li> Improper use of antibiotics </li>
 </ul><br>

<li> Linked to a large number of diseases </li>
 <ul>
  <li> Obesity, Diabetes </li>
  <li> Asthma, Allergies </li>
  <li> Crohn's disease, Ulcerative colitis </li>
  <li> Cancer, IBS, Autism </li>
 </ul>

</div>

<div class="right">
![unbalanced scale-50](2018-GalaxyEU/images/dysbiosis-balance.png)
![diseases](2018-GalaxyEU/images/microbiota-disease.jpg)

</div>

---

Improper antibiotics use can lead to dysbiosis

<div class="block">
<div class="three-left small">
![healthy forest](2018-GalaxyEU/images/forest-healthy.jpg)
Healthy gut
</div>
<div class="three-middle small">
![after antibiotics](2018-GalaxyEU/images/forest-burnt.jpg)
Gut after antibiotics
</div>
<div class="three-right small">
![monoculture](2018-GalaxyEU/images/forest-monoculture.jpg)
Monoculture
</div>
</div>

Note:
Antibitics kill gut


---


### Streeklab Haarlem

<div class="left small alignleft">

<br><br>
<ul>
<li> Microbial Diagnostics Laboratory</li><br>
<li> Services large number of </li>
 <ul>
  <li> Hospitals </li>
  <li> Clinics </li>
  <li> GPs </li>
 </ul><br>
<li>Samples (e.g. blood, stool, urine) are sent to the lab and analysed</li>
 <ul>
   <li> Determine microbiota present </li>
   <li> Determine antibiotic resistance </li>
   <li> Advise a treatment </li>
 </ul>
</ul>

</div>

<div class="right center">

![](2018-GalaxyEU/images/slh-logo2.png)
![](2018-GalaxyEU/images/slh-envelope.png)

</div>

---

### Streeklab Haarlem

<div class="left small">
<ul>
 <li>Samples are cultured</li><br>
 <li>Species determined by </li>
  <ul>
   <li> MALDI-TOF MS</li>
   <li> Visual inspection</li>
  </ul><br>
 <li>Limitations</li>
  <ul>
   <li> Medium determines what grows</li>
   <li> Some species difficult to culture</li>
  </ul><br>
 <li>Pilot study: 16S rRNA sequencing</li>
   <ul>
   <li> Can this augment current practices?</li>
  </ul>
</ul>

</div>
<div class="right">
![](2018-GalaxyEU/images/slh-culture.jpg)
</div>

---

### Experiment Design

Micelle

3 replicates
background control

Illumina MiSeq

---

### NGS Approaches

- Shotgun sequencing
- Amplicon sequencing

---

### Shotgun Sequencing

<div class="left small">
<ul>
<li> Sequence everything </li><br>
<li> Expensive ($1000+ per sample) </li><br>
<li> More information
 <ul>
  <li> Functional prediction</li>
  <li> Antibiotic resistance </li>
  <li> Unknown organisms </li>
</ul><br>
<li> Higher complexity </li>
</ul>
</div>

<div class="right">
![](2018-GalaxyEU/images/shotgun-puzzles.png)
</div>

---

### Amplicon Sequencing

<div class="left small">
<br>
<ul>
<li> Targetted approach </li>
  <ul>
   <li> 16S/18S rRNA gene </li>
   <li> Present in all bacteria and archaea </li>
  </ul></br>
<li>No contamination from: </li>
  <ul>
   <li>Host</li>
   <li>Environmental fungi, plants</li>
 </ul>
</ul>
</div>

<div class="right">
![](2018-GalaxyEU/images/16S-gene-ecoli.png)
</div>
---

### 16S rRNA gene

<div class="left small">
<ul>
 <!--<li> Ribosomal RNA gene </li>
 <ul>
   <li>~1500 bp long</li>
 </ul><br>-->
 <li> Highly conserved regions</li>
  <ul>
   <li>easy to target across all bacteria</li>
  </ul><br>
<li>Variable regions</li>
 <ul>
  <li>V1, V2,.., V9 </li>
  <li>distinguish between different bacteria</li>
 </ul>
</ul>
<br>
![](2018-GalaxyEU/images/16S_variableregions.jpg)
</div>

<div class="right">
![scale-70](2018-GalaxyEU/images/16S-structure.jpg)
</div>

Note:
- 16S gene is around 1500 nucleotides long
- Strong secondary structure, folds into 3D structure
- S stands for Svedberg (unit of time, time it takes to sediment in centrifuge)

---

### Amplicon Sequencing

<div class="left small">
<br>
<ul>
<li>Pros:</li>
 <ul>
  <li>Cheap: ($50-$100 per sample)</li>
  <li>Well-established</li>
  <li>Lot of reference databases</li>
 </ul> <br>
<li>Cons: </li>
  <ul>
  <li>Choice of V-region can bias results</li>
  <li>Difficult to resolve species/strains</li>
  </ul>
</ul>
</div>

<div class="right tiny">
![](2018-GalaxyEU/images/bias-vregions.png)
doi:10.1038/nature11209
</div>

Note:
Image: number of OTUs identified by genus for V13 region (y-axis)
and V35 region (x-axis)

For example for Coprococcus, 65 OTUs identified when using V35 region,
3 OTUs with V13 region.

---

### Streeklab Haarlem


![scale-70](2018-GalaxyEU/images/16S_end-to-end.png)
![scale-50](2018-GalaxyEU/images/so_much_data.png)

---

### Galaxy!

![](2018-GalaxyEU/images/workflow.png)

---

### Pipeline

![](2018-GalaxyEU/images/analysis_pipeline.png)

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



---

### OTU Clustering

**OTU**: Operational Taxonomic Unit

<div class="left">
![](2018-GalaxyEU/images/otu-clusters.png)
</div>
<div class="right">
![](2018-GalaxyEU/images/otu.png)
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

calculate alpha diversity for randomly selected subset of sequences in each sample

---

### Alpha Diversity

Diversity *within* a sample

- naive: just number of OTUs
- doesnt take into account relatedness of OTUs
- doesnt take into account relative disstribution
   - 3 species at 98%,1%,1%
   - 3 species at 33%,33%,33%

- As many diversity measures as there are ambitious ecologists
   - shannon, chao, .. ..

---

### Beta Diversity

Diversity *between* samples

---

### Visualisations

---

### Krona

---

### Phinch

mothur, Qiime, picrust

Phinch, krona, venn, heatmaps

---

### Results



---

### Training Materials


---

### Acknowledgements

<div class="left small">
<ul>
 <li>ErasmusMC Bioinformatics</li>
 <ul>
  <li>Andrew Stubbs</li>
  <li>Saskia Hiltemann</li>
  <li>Youri Hoogstrate</li>
  <li>David van Zessen</li>
  <li>Yunlei Li</li>
 </ul>
<br>
<li>ErasmusMC Clinical Microbiology</li>
 <ul>
  <li>John Hays</li>
  <li>Stefan Boers</li>
 </ul>
 <br>
<li>**Streeklab Haarlem**</li>
 <ul>
  <li>John Hays</li>
  <li>Stefan Boers</li>
 </ul>
</ul>
</div>
<div class="right">

</div>

---


---

### Mothur vs Qiime


---

### RDP classifier

- training data
- naive bayes
- kmer based

- confidence level: bootstrap

---

### Culture

- Bacteria grown on selective medium
- Bacteria determined by MALDI-TOF MS or eyeballed/biochemically
- MALDI: Matrix Assisted Laser Desorption/Ionization
- TOF MS: Time of Flight Mass Spectrometry
- Not all bacteria thrive equally (or at all) on medium
    - optimized to quickly show known pathogens
       - but "rest" can also be interesting
    - anaerobic bacteria are hard to grow in lab
- 16S cannot show antibiotic resistance, and only reliable down to genus level
- 16S usually equally quick
   - 16S 2-3 days
   - cultures: mostly 24-48 hours, some types difficult to culture and can take 2 weeks
- Costs: NGS higher, but when culture is negative, cheaper than hospitalization








