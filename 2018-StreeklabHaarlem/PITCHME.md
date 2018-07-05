# Data Analyse met Galaxy

Saskia Hiltemann

Juli 2018, Streeklab Haarlem

---

### Over Mij

<div class="left small">
<br><br><br>
<ul>
<li> Erasmus MC</li> <br>
<li> Bioinformatica groep (afdeling pathologie)</li><br>
<li> Analyse pipelines bouwen</li>
 <ul>
 <li> Gebruikers vriendelijk</li>
 <li> Onderzoeker/ Clinici *zelf* analyse kunnen uitvoeren</li>
 </ul><br>
<li> Prostaatkanker, Metagenomics, RNA-Seq, Immunologie </li>
</ul>
</div>

<div class="right">

![scale-60](assets/images/erasmusmc/logo-emc.png)
![scale-60](assets/images/erasmusmc/erasmusmc.jpg)

</div>
---

### Overview

- Wat is Galaxy?
- MYcrobiota pipeline
- HLA-DQ pipeline

---

### Bioinformatica: de moeilijk manier

Een `mothur` analyse op the linux command-line:

![scale-70](assets/images/microbiota/mothur_commandline.png)

Note:
-
- especially for non-programmers
- want to enable researchers and clinicians to run their own analyses

---

![](assets/images/galaxy/galaxy_logo.png)

<div class="left small">
<ul>
<li> Grafische schil om linux tools</li><br>
<li> Web-based (geen installatie nodig)</li><br>
<li> Grote gebruikers community</li>
  <ul>
  <li> meer dan 6000 tools</li>
  <li> meer dan 5500 publicaties</li>
  <li> meer dan 90 publieke servers</li>
  </ul><br>
<li> Nadruk op reproduceerbaarheid</li><br>
<li> Gratis & Open-Source</li>
</ul>
</div>

<div class="right">
![](assets/images/galaxy/galaxy_interface.png)
https://galaxyproject.org
</div>

---

### De Galaxy Interface


![](assets/images/galaxy/galaxy_instance_detailed_screenshot.png)

---

### De Galaxy manier

Een `mothur` commando in Galaxy:

<div class="left">
![](assets/images/microbiota/mothur_commandline.png)

</div>
<div class="right">
![](assets/images/galaxy/mothur_tool_interface.png)
</div>
---

### Data Uploaden

<div class="left small">
<ul>
<li>Data Knippen/Plakken</li>
<li>Bestanden van computer uploaden</li>
<li>Bestanden van internet importeren via url</li>
<li>Data Importeren van online databases</li>
<ul><li>UCSC, NCBI, ENA, BioMart, ENCODE, ..</li></ul>
<li> FTP voor zeer grote files</li>
</ul>
</div>
<div class="right">
![](assets/images/galaxy/upload_menu.png)
</div>

Note:
Allemaal in de browser

---

### Analyse Geschiedenis

<div class="left small">
<ul>
<li> Data bekijken, metadata aanpassen </li><br>
<li> Galaxy houdt analyse historie exact bij</li>
  <ul>
  <li> Tools & versies</li>
  <li> Parameter settings</li>
  <li> Input en referentie datasets</li>
  </ul><br>
<li> Kleuren geven status aan </li>
  <ul>
  <li> <a style="background-color: gray; color: white;">Grijs:</a> in de wachtrij </li>
  <li> <a style="background-color: yellow; color: black;">Geel:</a> taak is nu bezig </li>
  <li> <a style="background-color: green; color: white;">Groen:</a> succesvol voltooid </li>
  <li> <a style="background-color: red; color: white;">Rood:</a> fout opgetreden </li>
  </ul><br>
<li> Download, run info, herstart, visualisaties </li>
</ul>
</div>
<div class="right">
![scale-30](assets/images/galaxy/history.png)
</div>

---

### Analyse Geschiedenis

Zoveel histories als je wilt (vaak 1 per sample/run)

![](assets/images/galaxy/history_multiview.png)

Note:
- Switchen tussen histories
- Datasets verslepen tussen histories

---

### Workflows

Tools kunnen makkelijk gecombineerd worden tot analyse pipelines met de *workflow editor*

![scale-80](assets/images/galaxy/workflow_editor.png)

---

### Workflows

Workflow starten

![scale-70](2018-StreeklabHaarlem/images/hladq_workflow_run.png)



---


### Visualisaties

- Ingebouwde Genome browser
- Connecties met online visualisatie servers
- Tools die visualisaties produceren (bijv. Krona)

![scale-40](assets/images/microbiota/krona.png)

---

### iReport

- Tool in Galaxy die resultaat rapporten kan maken

![scale-60](assets/images/microbiota/mothur_ireport.png)


---

### Deel je werk

<div class="left">
<ul>
<li> Datasets, Histories, Workflows, Visualisaties</li>
  <ul>
  <li> Bepaalde gebruikers</li>
  <li>Alle gebruikers op server</li>
  <li>Openbaar</li>
  </ul>
</ul>
</div>
<div class="right">
![](assets/images/galaxy/shared_data.png)
</div>
---

### Galaxy Training

Centrale verzameling van Galaxy Training materialen

![scale-50](assets/images/galaxy/training_materials_website.png)

https://training.galaxyproject.org

---

### Demo Time

https://bioinf-ttt.erasmusmc.nl/galaxy/

https://bioinf-galaxian.erasmusmc.nl/galaxy/

https://usegalaxy.eu

---

### Streeklab Haarlem Pipelines

1. Microbioto Analyse
3. HLA-DQ

---?image=2018-GalaxyEU/images/background.jpg

<h2 style="color: white;"> Microbiota Analyse in Galaxy </h2>

---

### Human Microbiome


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

![](assets/images/microbiota/human_microbiome.png)

</div>
</div>

Sometimes referred to as your **second genome**


---
## MYcrobiota: Experimental Design

<div class="left small">

<ul>
 <li> Illumina MiSeq </li>
 <li> 16S rRNA Amplicon Sequencing</li>
 <li> Micelle PCR </li>
 <br>
 <li> 3 technische replicaten per sample </li>
 <li> 1 Negatief controle sample </li>
   <ul><li>correctie voor achtergrond contamination</li></ul>
 <li> 1 Intern controle sample </li>
  <ul>
   <li>bekend organisme in bekende hoeveelheid</li>
   <li>aantal kopieen afleiden (Micelle PCR)</li>
 </ul>
</ul>
</div>

<div class="right">
![](assets/images/microbiota/miseq.png)

</div>

---

### NGS Approaches

- Shotgun sequencing
- Amplicon sequencing

---

### Shotgun Sequencing

<div class="left small">
<ul>
<li> Alles Sequencen </li><br>
<li> Duur ($1000+ per sample) </li><br>
<li> Meer informatie
 <ul>
  <li> Functionele prediction</li>
  <li> Antibiotica resistentie </li>
  <li> Onbekende organisms </li>
</ul><br>
<li> Hogere complexiteit </li>
</ul>
</div>

<div class="right">
![](assets/images/microbiota/shotgun-puzzles.png)
</div>

---

### Amplicon Sequencing

<div class="left small">
<br>
<ul>
<li> Targetted approach </li>
  <ul>
   <li> 16S/18S rRNA gen </li>
   <li> Aanwezig in alle bacteria en archaea </li>
  </ul></br>
<li>Geen contaminatie van: </li>
  <ul>
   <li>Gastheer </li>
   <li>Omgeving (fungi, planten, humaan) </li>
 </ul>
</ul>
![scale-50](assets/images/microbiota/16S-gene-ecoli.png)
</div>


<div class="right">
![](assets/images/microbiota/amplicon-puzzles2.png)
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
 <li> Sterk geconserveerde regios</li>
  <ul>
   <li>makkelijk te targetting in verschillende organismen</li>
  </ul><br>
<li>Variable regios</li>
 <ul>
  <li>V1, V2,.., V9 </li>
  <li>onderscheid maken tussen verschillende bacteria</li>
 </ul>
</ul>
<br>
![](assets/images/microbiota/16S_variableregions.jpg)
</div>

<div class="right">
![scale-70](assets/images/microbiota/16S-structure.jpg)
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
  <li>Goedkoper: ($50-$100 per sample)</li>
  <li>Well-established</li>
  <li>Veel referentie databases</li>
 </ul> <br>
<li>Cons: </li>
  <ul>
  <li>Keuze V-region can resultaat beinvloeden</li>
  <li>Moeilijk om species/strains te bepalen</li>
  </ul>
</ul>
</div>

<div class="right tiny">
![](assets/images/microbiota/bias-vregions.png)
doi:10.1038/nature11209
</div>

Note:
Image: number of OTUs identified by genus for V13 region (y-axis)
and V35 region (x-axis)

For example for Coprococcus, 65 OTUs identified when using V35 region,
3 OTUs with V13 region.

TODO: move bias image til after explanation of OTUs?

---

![scale-70](assets/images/microbiota/16S_end-to-end.png)
![scale-50](assets/images/microbiota/so_much_data.png)

---

### Galaxy!

![](assets/images/microbiota/workflow.png)

---

### Pipeline

![](assets/images/microbiota/analysis_pipeline.png)

---

### Tools in Galaxy


<div class="right30">
![scale-40](assets/images/microbiota/mothur-logo.png)
![scale-40](assets/images/microbiota/qiime-logo.png)
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
![scale-40](assets/images/microbiota/mothur-logo.png)

<ul>
<li> C++ </li>
<li> Reimplements methods</li>
<li> Visualisations mostly not included</li>
<li> Open Source </li>
</ul>

</div>

<div class="right small">
![scale-40](assets/images/microbiota/qiime-logo.png)

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

### Pre-processing

![scale-50](assets/images/microbiota/preprocessing.png)

- Data kan op veel manieren gefilterd en opgeschoond worden
- Afweging tussen kwaliteit en hoeveelheid information behoudt

---

### Chimera removal


<div class="left">
<br><br>
<ul>
<li>Griekse mythologie </li>
 <ul>
  <li>Hybride dieren</li>
 </ul><br>
 <li>Sequencing data </li>
 <ul>
  <li> Hybride sequenties </li>
  <li> Ontstaan tijdens PCR</li>
 </ul><br>
 <li> Correctie Methoden </li>
 <ul>
  <li>In Silico</li>
  <li>Micelle PCR</li>
 </ul>
</ul>
</div>

<div class="right">
![scale-40](assets/images/microbiota/chimera-animal.jpg)
<br>
![scale-80](assets/images/microbiota/chimeras.png)
</div>

+++

### Traditional PCR

![](assets/images/microbiota/16S_end-to-end_nomicelle.png)

<div class="small">
<ul>
<li>PCR in een enkel compartiment</li>
<li>bias due to differences in efficiency of 16S gene amplifications</li>
<li>Susceptible to chimera formation</li>
</ul>
</div>
+++

### Micelle PCR

![](assets/images/microbiota/16S_end-to-end_micelle.png)

<div class="left70 small">
<ul>
<li>Every DNA molecule amplified individually</li>
 <ul><li> ~10^10 compartments</li></ul>
<li>Addition of **internal control** for quantification</li>
  <ul><li>known species at known quantities</li></ul>
<li>Improves microbiota analyses (doi: 10.1038/srep14181)</li>
</ul>
</div>

<div class="right30">
![scale-70](assets/images/microbiota/micelle.png)
</div>


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
 <li>Algoritmes</li>
 <ul>
  <li>Hierarchical clustering</li>
  <li>Seed-based clustering</li>
  <li>Model-based clustering</li>
 </ul>
</ul>
</div>

<div class="right">
![](assets/images/microbiota/otu-clusters.png)
![](assets/images/microbiota/otu-clustering-reference-based.png)
</div>

Note:
OTU definition (taxonomy, sequence similarity, phylogeny)
clustering strategy (de novo, open reference, closed reference)
distance metrics (pairwise alignment, multiple alignment, alignment-free)
algorithm (hierarchical clustering, seed-based, model-based)

---

### Taxonomie Bepalen

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
![scale-70](assets/images/microbiota/taxonomic-classification.jpeg)
![](assets/images/microbiota/silva-greengenes.png)
</div>
</div>

<div class="tiny">
Comparison: [10.1186/s12864-017-3501-4]((https://doi.org/10.1186/s12864-017-3501-4), [10.1093/nar/gkn491](https://doi.org/10.1093/nar/gkn491)
</div>

Note:
- often done after OTU clustering, but not necessarily
- GreenGenes not updated since 2013

+++

### Assigning taxonomy

![](assets/images/microbiota/taxonomy-methods.jpeg)

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

![](assets/images/microbiota/otutable.png)

Note:
domain, kingdom, phylum, class, order, family, genus, species

+++

### Diversity metrics

- Alpha Diversity
- Beta Diversity

Note:
Alpha diversity: diversity within 1 sample
Beta diversity: diversity between samples

in our case: every patient considered on its own, so only alpha diversity
is considered.

+++

### Alpha Diversity

Diversity *within* a sample

![scale-90](assets/images/microbiota/alpha-diversity.png)


+++

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
![](assets/images/microbiota/phylogenetic-distance.png)
</div>

Note:
- PD: sum of branch lengths
- in our pipeline we report several diversity metrics


+++

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

![](assets/images/microbiota/rarefaction.gif)

Calculate diversity for randomly selected subset of sequences in each sample


---

### Post-processing

<div class="left small">
<ul>
<li>3 replicates</li>
 <ul><li>OTU moet in allen aanwezig zijn</li></ul>
 <br>
 <li>Negative Extraction Control Sample</li>
  <ul><li>achtergrond aftrekken</li></ul>
 <br>
 <li>Interne Controle Sample</li>
  <ul><li>relatieve hoeveelheden -> kopieen</li></ul>

</ul>
</div>

<div class="right">

![](assets/images/microbiota/negative-control.jpg)
</div>

Note:
- tetramix: equimolar mix of 4 species
- 2500 to 2.5 16S rRNA gene copies per bacterial species

Synthetic microbial community (SMC) samples tested comprised equimolar 16S rRNA gene copies derived from C. perfringens, S. aureus, H. influenzae, and M. catarrhalis and ranging from 2,500 to 2.5 16S rRNA gene copies per bacterial species. Averages of triplicate micPCR/NGS and triplicate traditional PCR/NGS results are shown in 100% stacked bars before and after correction for contaminating bacterial DNA. The correction of contaminating bacterial DNA comprises two steps: 1) eliminating OTUs that could not be reproducibly measured in triplicate experiments, and 2) subtracting 16S rRNA gene copies that were also quantified in triplicate measurements of a negative extraction control (NEC) sample. Values within bars represent the calculated number of 16S rRNA gene copies per bacterial OTU.i


---

### Krona

![scale-50](assets/images/microbiota/krona.png)

<div class="tiny">
doi: 10.1186/1471-2105-12-385
</div>
---

<embed src="https://marbl.github.io/Krona/examples/rdp.krona.html">

+++

### Phinch

![scale-70](assets/images/microbiota/phinch_overviewpage.png)

<div class="tiny">
doi: 10.1101/009944
</div>

Note:
- useful for multi-sample analyses


---

### iReport

![](assets/images/microbiota/ireport-mycrobiota.png)

---

### Results: Post-operative wounds

<div class="left">
![](assets/images/microbiota/cultures.png)
</div>


<div class="right">
![](assets/images/microbiota/miseq2.png)
</div>

<div style="color: rgba(0,0,0,0)">bla</div>

<div class="tiny center">
<table >
<tr><td>Taxonomy</td><td>CFU</td><td>%</td>   <td>Taxonomy</td><td>Copies</td><td>%</td></tr>
<tr><td>Skin flora</td><td>+</td><td>33%</td>  <td>Anaerobic bacteria (12)</td><td>251.692</td><td>87%</td> </tr>
<tr><td>Staphylococcus aureus</td><td>++</td><td>67%</td>   <td>Streptococcus</td><td>30.408</td><td>10%</td></tr>
<tr><td></td>                     <td></td>   <td></td>     <td>Staphylococcus aureus</td><td>8.960</td><td>3%</td></tr>
</table>
</div>
<br>

<div class="small">
<ul>
 <li>Anaerobe bacterien net zo makkelijk identificeren en kwantificeren als aerobe bacterien</li>
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
![](assets/images/microbiota/arthritis.png)
</div>


+++

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
![](assets/images/microbiota/arthritis.png)
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
![](assets/images/microbiota/arthritis.png)
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
![](assets/images/microbiota/arthritis.png)
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
![](assets/images/microbiota/arthritis.png)
</div>

+++

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
![](assets/images/microbiota/hipimplant.jpg)
</div>

---

### MYcrobiota: Conclusie

<div class="small">
<ul>
 <li>MYcrobiota biedt zeer nauwkeurige kwantitatieve microbiota analyses</li>
 <li>Kan inzicht bieden waar culturen negatief waren</li>
 <li>Geschikt voor samples met lage biomassa</li>
 <li>Clinici kunnen het gebruiken zonder tussenkomst van bioinformaticus</li>
</ul>
</div>
---

### Training Materials


![](assets/images/microbiota/training-material.png)

<div class="tiny">
https://training.galaxyproject.org
</div>


---?image=assets/images/streeklab-haarlem/immune_system.jpg

<h2 style="color: white;"> HLA-DQ pipeline </h2>

---

### De volledige pipeline

![](2018-StreeklabHaarlem/images/workflow_full-screenshot.png)

---

### De grote lijnen

- Per patient 2 paired-end samples (dus 4 input files)
  - HLADQ-A en HLADQ-B
- Forward en reverse reads combineren tot contigs
- Bepaal welke sequenties meest voorkomen
- BLAST met IMGT/HLA database
- Resultaten Rapporteren

---

### iReport

![](2018-StreeklabHaarlem/images/hladq_ireport_overview.png)

---

### iReport

![scale-50](2018-StreeklabHaarlem/images/hladq_ireport_tabB.png)


---

### Collecties

<div class="left small">
<br><br>
<ul>
<li>Eerste versie van de workflow vroeg om 4 inputs</li><br>
<li>Makkelijk A en B of forward/reverse perongeluk te verwisselen</li><br>
<li>Veel werk bij grote aantallen samples</li>
</ul>
</div>
<div class="right">
![](2018-StreeklabHaarlem/images/4inputs.png)
</div>
---

### Collecties

<div class="small">
<ul>
<li> Als je veel samples hebt1, kun je ze in Galaxy uploaden naar een *dataset collectie* </li>
<li>Als je nu een workflow start, wordt automatisch voor ieder sample in je collectie de workflow gerund </li>
</ul>
</div>

<div class="left">
![](assets/images/galaxy/collection_upload.png)
![](assets/images/galaxy/collection_history_item.png)

</div>
<div class="right">
![](2018-StreeklabHaarlem/images/1input.png)
</div>

---

### Collecties

<div class="left small">
<ul>
<li> Consitente naamgeving van files</li>
<li> <a style="font-size: 0.7em;"> `HLADQ[A|B]-<SID>_SXX_L001_R[1|2]_001.fastq` </a></li><br>
<li>Galaxy weet dan automatisch:</li>
  <ul>
  <li> welke forward/reverse files die bij elkaar horen</li>
  <li> welke A en B sample van die zelfde patient zijn</li>
  <li> minder kans op sample swap</li>
  </ul><br>
<li> Erg nieuwe feature in Galaxy</li>
  <ul>
  <li> "Rule Builder" </li>
  <li> Elana's pipeline gepresenteerd op de Galaxy conferentie vorige week door developer van die fearture :)</li>
  </ul>
</ul>
</div>

<div class="right">
![](2018-StreeklabHaarlem/images/rule_builder1.png)
![](2018-StreeklabHaarlem/images/workflow-screenshot.png)
</div>

Note:
johns presentation: https://docs.google.com/presentation/d/1MxFfMKINUMKat-bgb9NFDpbyRzwXWS0xNadJJW8llHk/edit#slide=id.g3807979e14_0_55
---

### Onze Servers en Services

---

### Servers

- TTT server: beheert door EMC, speciaal voor SLH
- Galaxian: beheerd door EMC, open voor iedereen in EMC
- GalaxyEU: beheerd door Freiburg, open voor iedereen in wereld
- GalaxyMain: beheerd door PennState, open voor iedereen in wereld


---

### Servers

- Relatief makkelijk om zelf een Galaxy te runnen
- Wij maken VM, Streeklab Haarlem draait deze lokaal
   - snellere data upload tijden
   - in eigen beheer, minder afhankelijk van EMC
   - backup server bij EMC om naar uit te wijken bij downtime

+++

### Servers


![](assets/images/galaxy/galaxian_uptime.png)

[https://stats.usegalaxy.eu](https://stats.usegalaxy.eu/d/000000020/public-galaxy-servers)

---

### Training

<div class="left small">
<ul>
<li>Ieder jaar een 2/3 daagse Galaxy training in EMC</li>
<ul><li>Volgende Editie in November</li></ul>
<li>17-19 October: Elixir Galaxy cursus in het VU</li>
<li>Galaxy workshop organiseren op Streeklab Haarlem?</li>
</ul></li>
</div>

<div class="right">
![](assets/images/galaxy/events.png)
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
![scale-30](assets/images/microbiota/slh-logo.jpg)
</div>

---

### Questions?

![](assets/images/questions.jpg)


---

### Galaksio?



