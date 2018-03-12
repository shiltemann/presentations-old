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

### Dysbiosis

Can be caused by improper use of antibiotics

<div class="block">
<div class="three-left small">
![healthy forest](2018-GalaxyEU/images/forest-healthy.jpg)
Healthy microbiome
</div>
<div class="three-middle small">
![after antibiotics](2018-GalaxyEU/images/forest-burnt.jpg)
After antibiotics
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

Note:
- MALDI: Matrix Assisted Laser Desorption/Ionization
- TOF MS: Time of Flight Mass spectrometry


---

### Experimental Design

<div class="left small">

<ul>
 <li> Illumina MiSeq </li>
 <li> 16S rRNA Amplicon Sequencing</li>
 <li> Micelle PCR </li>
 <br>
 <li> 3 technical replicates </li>
 <li> Negative control sample </li>
   <ul><li>correct background contamination</li></ul>
 <li> Internal control sample </li>
  <ul><li>estimate number of copies</li></ul>
</ul>
</div>

<div class="right">
![](2018-GalaxyEU/images/miseq.png)

</div>

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

TODO: move bias image til after explanation of OTUs?

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

### Tools in Galaxy


<div class="right30">
![scale-40](2018-GalaxyEU/images/mothur-logo.png)

![scale-40](2018-GalaxyEU/images/qiime-logo.png)
</div>

<div class="left70 small">
<ul>
<li> \> 250 tools in metagenomics category in Tool Shed </li><br>
<li> 2 large tool suites</li>
 <ul><li>Mothur</li><li>Qiime</li></ul><br>
<li> Visualisation tools </li>
 <ul>
  <li>Krona</li>
  <li>Phinch</li>
 </ul><br>
<li> PICRUSt </li>
 <ul><li>functional content prediction based on phylogeny</li></ul><br>
<li> .. </li>
</ul>
</div>

---

### Chimera removal


<div class="left small">
<br><br>
<ul>
<li>Greek mythology </li>
 <ul>
  <li>Hybrid animals</li>
 </ul><br>
 <li>Sequencing data </li>
 <ul>
  <li> Hybrid sequences </li>
  <li> Created during PCR</li>
 </ul><br>
 <li> Correction Methods </li>
 <ul>
  <li>In Silico</li>
  <li>Micelle PCR</li>
 </ul>
</ul>
</div>

<div class="right">
![scale-40](2018-GalaxyEU/images/chimera-animal.jpg)
<br>
![scale-80](2018-GalaxyEU/images/chimeras.png)
</div>

---

### Traditional PCR

![](2018-GalaxyEU/images/16S_end-to-end_nomicelle.png)

<div class="small">
<ul>
<li>PCR performed in single compartment</li>
<li>bias due to differences in efficiency of 16S gene amplifications</li>
<li>Susceptible to chimera formation</li>
</ul>
</div>
---

### Micelle PCR

![](2018-GalaxyEU/images/16S_end-to-end_micelle.png)

<div class="left70 small">
<ul>
<li>Every DNA molecule amplified individually</li>
 <ul><li> ~10^10 compartments</li></ul>
<li>Addition of **internal control** for quantification</li>
<li>Improves microbiota analyses (doi: 10.1038/srep14181)</li>
</ul>
</div>

<div class="right30">
![scale-70](2018-GalaxyEU/images/micelle.png)
</div>
---

### OTU Clustering

**OTU**: Operational Taxonomic Unit

<div class="left">
![](2018-GalaxyEU/images/otu-clusters.png)
</div>
<div class="right">
![](2018-GalaxyEU/images/otu.png)
</div>

Note:
- clusters of closely related sequences
- proxy for species/genus (97%=species, but perhaps not too reliable)
- control for sequencing/PCR errors
- for amplicon data, not done so much in shotgun
-

---

### OTU Clustering

3 main ways to do OTU picking:
  - De novo
  - Closed reference
  - Open reference


Note:
OTU definition (taxonomy, sequence similarity, phylogeny)
clustering strategy (de novo, open reference, closed reference)
distance metrics (pairwise alignment, multiple alignment, alignment-free)
algorithm (hierarchical clustering, seed-based, model-based)


---

### Distance Metrics

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

### Assigning Taxonomy

SILVA, greengenes

---

### Post-processing

3 replicates
- OTU must be present in all of them
- subtract background sample ("empty sample")
- relative abundance -> copies (using internal control)

---

### Visualisations

---

### Krona

![scale-50](2018-GalaxyEU/images/krona.png)

<div class="tiny">
doi: 10.1186/1471-2105-12-385
</div>
---

<embed src="https://marbl.github.io/Krona/examples/rdp.krona.html">

---

### Phinch

![scale-70](2018-GalaxyEU/images/phinch_overviewpage.png)

<div class="tiny">
doi: 10.1101/009944
</div>


---

### iReport

![](2018-GalaxyEU/images/ireport-mycrobiota.png)

---

### Results: Case 1


<div class="left small">
<li>Arthritis patient</li>
<li>History of dental extraction</li>
<li>Culture negative</li>

<li>Result: Prevotella denticola - 70.000 copies</li>
 <ul>
  <li>typical inhabitant of the oral flora</li>
  <li>Hard to culture under standard conditions</li>
 </ul>
</div>

<div class="right">
![](2018-GalaxyEU/images/arthritis.png)
</div>


---

### Results

CASE 2:

- Arthritis patient
- History: operation of the intestine
- Culture negative

- Rhuminococcus species - 192.000 copies
  - Inhabitant of the intestine
  - Hard to culture under standard conditions

---

### Results

CASE 3:

- Infected hip implant
- 5 samples from different locations
- No culture data available

- Staphylococcus - 3, 53, 10, 742, 1072K gene copies
  - most likely contaminations during operation

---

### Training Materials


![](2018-GalaxyEU/images/training-material.png)

<div class="tiny">
https://training.galaxyproject.org
</div>


---

### Acknowledgements

<div class="left small">
<br>
<ul>
 <li>**ErasmusMC Bioinformatics**</li>
 <ul>
  <li>Andrew Stubbs</li>
  <li>Saskia Hiltemann</li>
  <li>Youri Hoogstrate</li>
  <li>David van Zessen</li>
  <li>Yunlei Li</li>
 </ul>
<br>
<li>**ErasmusMC Clinical Microbiology**</li>
 <ul>
  <li>John Hays</li>
  <li>Stefan Boers</li>
 </ul>
 <br>
<li>**Streeklab Haarlem**</li>
 <ul>
  <li>Ruud Jansen</li>
  <li>Elana Meijer</li>
 </ul>
</ul>
</div>
<div class="right">
![scale-50](assets/images/logo-emc.png)
<br>
![scale-30](2018-GalaxyEU/images/slh-logo.jpg)
</div>

---


---

### Mothur vs Qiime


<div class="block">
<div class="left small">
![scale-40](2018-GalaxyEU/images/mothur-logo.png)

<ul>
<li> C++ </li>
<li> reimplements methods</li>
<li> visualisations mostly not included</li>
<li> Open Source </li>
</ul>

</div>

<div class="right small">
![scale-40](2018-GalaxyEU/images/qiime-logo.png)

<ul>
<li>python</li>
<li>wraps existing methods </li>
<li>better visualisations </li>
<li> Open Source, but wraps some closed-source components </li>
</ul>
</div>
</div>

http://blog.mothur.org/2016/01/12/mothur-and-qiime/

Note:

- both work well and are very similar
- comes down to personal preference
- qiime better visualisations, but works with biom so can use it on mothur data as well
- qiime2 released as VM, packaging more difficult

---

### RDP classifier

- training data
- naive bayes
- kmer based

- confidence level: bootstrap

---

### Culture

<div class="small">
<ul>
<li>Bacteria grown on selective medium</li>
<li> Bacteria determined by MALDI-TOF MS or eyeballed/biochemically</li>
 <ul>
  <li> MALDI: Matrix Assisted Laser Desorption/Ionization</li>
  <li> TOF MS: Time of Flight Mass Spectrometry</li>
 </ul>
<li> Not all bacteria thrive equally (or at all) on medium</li>
 <ul>
   <li> optimized to quickly show known pathogens</li>
   <li> but "rest" can also be interesting</li>
   <li> anaerobic bacteria are hard to grow in lab</li>
 </ul>
<li> 16S cannot show antibiotic resistance, and only reliable down to genus level</li>
<li> 16S usually equally quick</li>
 <ul>
  <li> 16S 2-3 days</li>
  <li> cultures: mostly 24-48 hours, some types difficult to culture and can take 2 weeks</li>
 </ul>
<li> Costs: NGS higher, but when culture is negative, cheaper than hospitalization</li>
</ul?
</div>






