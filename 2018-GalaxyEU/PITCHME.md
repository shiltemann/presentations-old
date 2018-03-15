---?image=2018-GalaxyEU/images/background.jpg

<div class="white">
<h2 class="white"> Microbiota Analysis using Galaxy </h2>

Saskia Hiltemann

</div>

---

### Overview

- Background 16S rRNA sequencing
- Streeklab Haarlem
- Analysis pipeline
- Clinical Results

Note:

I will start with a general introduction to 16S rRNA amplicon sequencing

then tell you a bit about a collaboration we have with a diagnostics lab called Streeklab Haarlem

and show you the pipeline we built in Galaxy for their use case

and finally show some of the results from our pilot study with them to bring 16S rRNA sequencing to the clinic

+++

### Microbiota

![Video](https://www.youtube.com/embed/htbeJhtFAXw)

+++

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


+++

Pasteur: Food spoilage
von Koch: Germ theory

---

### Why study the microbiome?


<div class="block">
<div class="left small middle">
<br><br>
<ul>
  <li>Humans are full of micro-organisms</li>
  <ul>
   <li> Skin, gut, oral cavity, lungs, eyes, ..</li>
   <li> Impacting health, drug efficacy </li>
  </ul>
  <br>
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

Note:

- many applications in ecology
  - soil analysis -> agriculture

- as a hospital, we are interested in humans
- humans are also full of microorganisms
  - e.g. skin, gut, oral and nasal cavities, lungs, even eyes
  - impact on health and drug efficacy


---


### Dysbiosis

<div class="block">
<div class="left small leftalign">

<ul>
<li> Microbial imbalance in the body </li>
<ul><li>Symbionts, Commensals, Pathobionts</li></ul>
<br>

<li> Causes </li>
 <ul>
  <li> Infection  </li>
  <li> Lifestyle (diet, stress) </li>
  <li> Host genetics </li>
  <li> Medications </li>
 </ul><br>

<li> Linked to a large number of diseases </li>
 <ul>
  <li> Obesity, Diabetes </li>
  <li> Asthma, Allergies </li>
  <li> Crohn's disease, Ulcerative colitis </li>
  <li> Cancer, IBS, Autism </li>
 </ul>

</div>

<div class="right tiny">
![unbalanced scale-50](2018-GalaxyEU/images/dysbiosis-balance.png)
![diseases](2018-GalaxyEU/images/microbiota-disease.jpg)

</div>
</div>

<div class="tiny">
doi:10.1038/nri2515
</div>

Note:

Dysbiosis is a general term for an imbalance in your body's microbiome

A healthy microbiota contains a balanced composition
of many classes of bacteria.

**Symbionts** are organisms with known health-
promoting functions.

**Commensals** are permanent residents of this complex ecosystem and provide no benefit
or detriment to the host (at least to our knowledge).

**Pathobionts** are also permanent residents of the microbiota
and have the potential to induce pathology.

with **dysbiosis** there is an unnatural shift in the composition of
the microbiota, which results in either a reduction in the
numbers of symbionts and/or an increase in the numbers
of pathobionts.

The causes for this are not entirely clear,
but are likely to include recent societal advances in
developed countries. The result is non-specific inflammation,
which may predispose certain genetically susceptible
people to inflammatory disease and may be caused by
pathogens, which are opportunistic organisms that cause
acute inflammation.

+++

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
There are many causes of dysbiosis, but one of thm is improper use of antibiotics

Imaging a healthy microbiome as a lush, green rainforest

When you administer antibiototics it is as if you burn this forest to the ground

But this can lead to a situation where a single species can


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
 <li>Pilot study: MYcrobiota</li>
   <ul>
   <li> 16S rRNA sequencing</li>
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

### MYcrobiota: Experimental Design

<div class="left small">

<ul>
 <li> Illumina MiSeq </li>
 <li> 16S rRNA Amplicon Sequencing</li>
 <li> Micelle PCR </li>
 <br>
 <li> 3 technical replicates per sample </li>
 <li> 1 Negative control sample </li>
   <ul><li>correct background contamination</li></ul>
 <li> 1 Internal control sample </li>
  <ul>
   <li>known species at a known quantity</li>
   <li>estimate number of copies</li>
 </ul>
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
![scale-50](2018-GalaxyEU/images/16S-gene-ecoli.png)
</div>


<div class="right">
![](2018-GalaxyEU/images/amplicon-puzzles2.png)
</div>

Note:
- where shotgun was looking at whole puzzle, this is more like
  looking at only topleft corner of each puzzle

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

+++

### Mothur vs Qiime


<div class="block">
<div class="left small">
![scale-40](2018-GalaxyEU/images/mothur-logo.png)

<ul>
<li> C++ </li>
<li> Reimplements methods</li>
<li> Visualisations mostly not included</li>
<li> Open Source </li>
</ul>

</div>

<div class="right small">
![scale-40](2018-GalaxyEU/images/qiime-logo.png)

<ul>
<li>Python</li>
<li>Wraps existing methods </li>
<li>Better visualisations </li>
<li>Open Source, but wraps some closed-source components </li>
</ul>
</div>
</div>

http://blog.mothur.org/2016/01/12/mothur-and-qiime/

Note:

- both work well and are very similar
- comes down to personal preference
- mothur faster cuz C/C++
- qiime better visualisations, but works with biom so can use it on mothur data as well
- qiime proprietary components (e.g. USEARCH)

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
<li>Addition of **Negative control**</li>
  <ul><li>remove background contamination</li></ul>
<li>Addition of **internal control** for quantification</li>
  <ul><li>known species at known quantities</li></ul>
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
- proxy for species/genus (97%=species, but perhaps too close to sequencing error territory to be reliable)
- control for sequencing/PCR errors
- for amplicon data, this is not done so much in shotgun
-

---

### OTU Clustering

<div class="left small">
<ul>
 <li>Clustering Approaches:</li>
 <ul>
  <li>De novo</li>
 </ul>
</ul>
</div>

<div class="right">
![](2018-GalaxyEU/images/otu-clusters.png)
![](2018-GalaxyEU/images/otu-clustering-reference-based-placeholder.png)
</div>

Note:
OTU definition (taxonomy, sequence similarity, phylogeny)
clustering strategy (de novo, open reference, closed reference)
distance metrics (pairwise alignment, multiple alignment, alignment-free)
algorithm (hierarchical clustering, seed-based, model-based)

---

### OTU Clustering

<div class="left small">
<ul>
 <li>Clustering Approaches:</li>
 <ul>
  <li>De novo</li>
  <li>Closed reference</li>
 </ul>
</ul>
</div>

<div class="right">
![](2018-GalaxyEU/images/otu-clusters.png)
![](2018-GalaxyEU/images/otu-clustering-reference-based.png)
</div>

Note:
OTU definition (taxonomy, sequence similarity, phylogeny)
clustering strategy (de novo, open reference, closed reference)
distance metrics (pairwise alignment, multiple alignment, alignment-free)
algorithm (hierarchical clustering, seed-based, model-based)


---

### OTU Clustering

<div class="left small">
<ul>
 <li>Clustering Approaches:</li>
 <ul>
  <li>De novo</li>
  <li>Closed reference</li>
  <li>Open Reference</li>
 </ul>
</ul>
</div>

<div class="right">
![](2018-GalaxyEU/images/otu-clusters.png)
![](2018-GalaxyEU/images/otu-clustering-reference-based.png)
</div>

Note:
OTU definition (taxonomy, sequence similarity, phylogeny)
clustering strategy (de novo, open reference, closed reference)
distance metrics (pairwise alignment, multiple alignment, alignment-free)
algorithm (hierarchical clustering, seed-based, model-based)

---


### OTU Clustering

<div class="left small">
<ul>
 <li>Clustering Approaches:</li>
 <ul>
  <li>De novo</li>
  <li>Closed reference</li>
  <li>Open reference</li>
 </ul>
 <br>
 <li>Distance Metrics</li>
 <ul>
  <li>Pairwise alignment</li>
  <li>Multiple alignment</li>
  <li>Alignment-free</li>
 </ul>
 <br>
 <li>Algorithms</li>
 <ul>
  <li>Hierarchical clustering</li>
  <li>Seed-based clustering</li>
  <li>Model-based clustering</li>
 </ul>
</ul>
</div>

<div class="right">
![](2018-GalaxyEU/images/otu-clusters.png)
![](2018-GalaxyEU/images/otu-clustering-reference-based.png)
</div>

Note:
OTU definition (taxonomy, sequence similarity, phylogeny)
clustering strategy (de novo, open reference, closed reference)
distance metrics (pairwise alignment, multiple alignment, alignment-free)
algorithm (hierarchical clustering, seed-based, model-based)

---

### Assigning Taxonomy

<div class="block">
<div class="left small">
<ul>
 <li>Methods</li>
 <ul>
  <li>Sequence alignment</li>
  <li>K-mer based methods</li>
  <li>Tree based methods</li>
  <li>Machine learning</li>
 </ul>
 <br>
 <li>Reference Databases</li>
 <ul>
  <li>SILVA</li>
  <li>Green Genes</li>
  <li>RDP</li>
  <li>NCBI</li>
 </ul>
</ul>
</div>

<div class="right">
![scale-70](2018-GalaxyEU/images/taxonomic-classification.jpeg)
![](2018-GalaxyEU/images/silva-greengenes.png)
</div>
</div>

<div class="tiny">
Comparison: [10.1186/s12864-017-3501-4]((https://doi.org/10.1186/s12864-017-3501-4), [10.1093/nar/gkn491](https://doi.org/10.1093/nar/gkn491)
</div>

Note:
- often done after OTU clustering, but not necessarily
- GreenGenes not updated since 2013

---

### Assigning taxonomy

![](2018-GalaxyEU/images/taxonomy-methods.jpeg)

<div class="tiny">
doi: 10.1093/nar/gkn491
</div>

Note:

- composition at phylym level
- each box a different dataset
- each subpanel (row) a different clasisfication method
- x-axis: region sequenced
- y-axis: abundance as fraction of total
- conclusion: choice of classifier has great impact on species identified

figure legend:
Compositions at the phylum level for each of the three datasets: (a) Guerrero Negro mat, (b) Human gut and (c) Mouse gut, using a range of different methods (separate subpanels within each group). The x-axis of each graph shows region sequenced. The y-axis shows abundance as a fraction of the total number of sequences in the community. The legend shows colors for phyla (consistent across graphs).

---

### OTU table

![](2018-GalaxyEU/images/otutable.png)

Note:
domain, kingdom, phylum, class, order, family, genus, species

---

### Diversity metrics

- Alpha Diversity
- Beta Diversity

Note:
Alpha diversity: diversity within 1 sample
Beta diversity: diversity between samples

in our case: every patient considered on its own, so only alpha diversity
is considered.

---

### Alpha Diversity

Diversity *within* a sample

![scale-90](2018-GalaxyEU/images/alpha-diversity.png)


---

### Alpha Diversity


<div class="small left70">
<ul>
 <li>Simple approach: count number of OTUs</li>
 <br>
 <li>Doesnt take into account relatedness of OTUs</li>
  <ul><li>Phylogenetic distance metrics</li></ul>
 <br>
 <li>Doesnt take into account relative distribution</li>
 <ul>
  <li>Sample A: 3 species at 98%,1%,1%</li>
  <li>Sample B: 3 species at 33%,33%,33%</li>
 </ul>
</ul>
</div>

<div class="right30">
![](2018-GalaxyEU/images/phylogenetic-distance.png)
</div>

Note:
- PD: sum of branch lengths
- in our pipeline we report several diversity metrics


---

### Diversity

<div class="block small">
*"As many diversity measures as there are ambitious ecologists"*
<br><br>
shannon, chao, pd, ace, simpson, sobs, jack, npshannon, smithwilson, heip
bergerparker, boney, efron, shen, solow, bootstrap, qstat, coverage, anderberg,
hamming, jclass, jest, ochiai, canberra, thetayc, invsimpson, ...
</div>


<div class="small">
https://www.mothur.org/wiki/Calculators
</div>

---

### Rarefaction

Have I captured the full diversity of my sample?

![](2018-GalaxyEU/images/rarefaction.gif)

calculate alpha diversity for randomly selected subset of sequences in each sample


---

### Post-processing

<div class="left small">
<ul>
<li>3 replicates</li>
 <ul><li>OTU must be present in all of them</li></ul>
 <br>
 <li>Negative Extraction Control Sample</li>
  <ul><li>subtract background sample</li></ul>
 <br>
 <li>Internal Control Sample</li>
  <ul><li>relative abundance -> copies</li></ul>

</ul>
</div>

<div class="right">

![](2018-GalaxyEU/images/negative-control.jpg)
</div>

Note:
- tetramix: equimolar mix of 4 species
- 2500 to 2.5 16S rRNA gene copies per bacterial species

Synthetic microbial community (SMC) samples tested comprised equimolar 16S rRNA gene copies derived from C. perfringens, S. aureus, H. influenzae, and M. catarrhalis and ranging from 2,500 to 2.5 16S rRNA gene copies per bacterial species. Averages of triplicate micPCR/NGS and triplicate traditional PCR/NGS results are shown in 100% stacked bars before and after correction for contaminating bacterial DNA. The correction of contaminating bacterial DNA comprises two steps: 1) eliminating OTUs that could not be reproducibly measured in triplicate experiments, and 2) subtracting 16S rRNA gene copies that were also quantified in triplicate measurements of a negative extraction control (NEC) sample. Values within bars represent the calculated number of 16S rRNA gene copies per bacterial OTU.i


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

Note:
- useful for multi-sample analyses


---

### iReport

![](2018-GalaxyEU/images/ireport-mycrobiota.png)

---

### Results: Post-operative wounds

<div class="left">
![](2018-GalaxyEU/images/cultures.png)
</div>


<div class="right">
![](2018-GalaxyEU/images/miseq2.png)
</div>

<div class="tiny">
<table>
<tr><td>Taxonomy</td><td>CFU</td><td>%</td>   <td>Taxonomy</td><td>Copies</td><td>%</td></tr>
<tr><td>Skin flora</td><td>+</td><td>33%</td>  <td>Anaerobic bacteria (12)</td><td>251.692</td><td>87%</td> </tr>
<tr><td>Staphylococcus aureus</td><td>++</td><td>67%</td>   <td>Streptococcus</td><td>30.408</td><td>10%</td></tr>
<tr><td></td>                     <td></td>   <td></td>     <td>Staphylococcus aureus</td><td>8.960</td><td>3%</td></tr>
</table>

</div>

<br>

<div class="small">
<ul>
 <li>Identify and quantify anaerobic bacteria just as easily as aerobic bacteria</li>
</ul>
</div>

Note:

CFU: Colony Forming Unit

---

### Results: Septic Arthritis

<div class="left70 small">
<ul>
 <li>19 patients</li>
 <li>Suspected septic arthritis</li>
 <li>Culture negative</li>

 <br>
 <li>MYcrobiota:</li>
 <ul>
  <li>confirmed 12/19 negative cultures</li>
  <li>detected bacteria in 7/19 negative cultures</li>
  <ul>
   <li>Parvimonasi, Prevotella, Ruminococcus</li>
   <li>Kingella -> confirmed with Kingella kingae specific PCR</li>
   <li>Ureaplasma </li>
   <li>Enterococus, Turicella</li>
  </ul>
 </ul>


</ul>
</div>

<div class="right30">
![](2018-GalaxyEU/images/arthritis.png)
</div>


---

### Results: Septic Arthritis


<div class="left70 small">
<ul>
<li>Suspected Septic Arthritis patient</li>
<li>History of dental extraction</li>
<li>Culture negative</li>
<br>

<li>MYcrobiota: Prevotella denticola</li>
 <ul>
  <li>70K copies</li>
  <li>typical inhabitant of the oral flora</li>
  <li>Hard to culture under standard conditions</li>
 </ul>
</ul>
</div>

<div class="right30">
![](2018-GalaxyEU/images/arthritis.png)
</div>


+++

### Results: Septic Arthritis 2

<div class="left70 small">
<ul>
<li>Arthritis patient</li>
<li>History: operation of the intestine</li>
<li>Culture negative</li>
<br>

<li>MYcrobiota: Rhuminococcus species</li>
  <ul>
  <li>192K copies</li>
  <li>Inhabitant of the intestine</li>
  <li>Hard to culture under standard conditions</li>
  </ul>
</ul>
</div>

<div class="right30">
![](2018-GalaxyEU/images/arthritis.png)
</div>

+++

### Results: Septic Arthritis 3

<div class="left70 small">
<ul>
<li>Arthritis patient</li>
<li>Culture Negative</li>
<br>
<li>MYcrobiota: Neisseria meningitidis</li>
 <ul>
  <li>895K copies</li>
  <li>inhabitant of the throat</li>
  <li>causative agent of bacterial meningitis</li>
  <li>probably not culturable due to use of antibiotics</li>
 </ul>

</ul>
</div>

<div class="right30">
![](2018-GalaxyEU/images/arthritis.png)
</div>

+++

### Results: Septic Arthritis 4

<div class="left70 small">
<ul>
<li>Arthritis patient</li>
<li>Culture Negative</li>
<br>
<li>Ureaplasma</li>
 <ul>
  <li>1200 copies</li>
  <li>not culturable in routine diagnostics</li>
 </ul>
</ul>
</div>

<div class="right30">
![](2018-GalaxyEU/images/arthritis.png)
</div>



---

### Results: Hip Transplant

<div class="left70 small">
<ul>
<li>Infected hip implant</li>
<li> 5 samples from different locations</li>
<li> No culture data available</li>
<br>
<li> Result: Staphylococcus </li>
  <ul>
  <li> 1.3K, 53K, 10K, 742K, 1072K gene copies</li>
  <li> most likely contaminations during operation</li>
  </ul>
</ul>
</div>
<div class="right30">
![](2018-GalaxyEU/images/hipimplant.jpg)
</div>

---

### Conclusion

<div class="small">
<ul>
 <li>MYcrobiota offers very precise quantitative microbiota analyses</li>
 <li>Can provide valuable insight in cases where cultures were negative</li>
 <li>Well suited for samples with low biomass</li>
 <li>Clinicians can use it without bioinformatics expertise needed</li>
</ul>
</div>
---

### Training Materials


![](2018-GalaxyEU/images/training-material.png)

<div class="tiny">
https://training.galaxyproject.org
</div>


---

### Acknowledgements

<div class="left tiny">
<br>
<ul>
 <li>**ErasmusMC Bioinformatics**</li>
 <ul>
  <li>Andrew Stubbs</li>
  <li>Saskia Hiltemann</li>
  <li>Youri Hoogstrate</li>
  <li>David van Zessen</li>
  <li>Yunlei Li</li>
  <li>Bas Horsman</li>
  <li>Rick Jansen</li>
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
  <li>Linda van de Nes-Reijnen</li>
  <li>Wil van der Reijden</li>
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






