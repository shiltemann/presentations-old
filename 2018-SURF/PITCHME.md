---?image=2018-GalaxyEU/images/background.jpg

<div class="white">
<h2 class="white"> Diagnostics with Galaxy: Microbiota Analysis </h2>

Saskia Hiltemann

</div>

---

### About Me

<div class="left small">
<br><br><br>
<ul>
<li> Erasmus MC</li> <br>
<li> Bioinformatics group (department of pathologie)</li><br>
<li> Build analysis pipelines</li>
 <ul>
 <li> User friendly</li>
 <li> Researchers/clinician should be able to run analyses themselves</li>
 </ul><br>
<li> Prostate Cancer, Metagenomics, RNA-Seq, Immunology </li>
</ul>
</div>

<div class="right">

![scale-60](assets/images/erasmusmc/logo-emc.png)
![scale-60](assets/images/erasmusmc/erasmusmc.jpg)

</div>


---

### Overview

- Introduction to Galaxy
- Introduction to Microbiota analyses
- Diagnostics pipeline for Streeklab Haarlem
- Run it in the SURF cloud?

Note:

Not using SURF's infra yet, but this project seems ideally suited

---

### What is Galaxy?

---

### Bioinformatics: the hard way

A `mothur` (metagenomics) analysis on the linux command-line:

![scale-70](assets/images/microbiota/mothur_commandline.png)


Note:

- especially for non-programmers
- want to enable researchers and clinicians to run their own analyses

---

![](assets/images/galaxy/galaxy_logo.png)

<div class="left small">
<ul>
<li> Graphical interface for linux tools</li><br>
<li> Web-based (no installatie required)</li><br>
<li> Large user community</li>
  <ul>
  <li> over 6000 tools</li>
  <li> over 5500 publications</li>
  <li> over 100 public servers</li>
  </ul><br>
<li> Emphasis on reproducibility </li><br>
<li> Free & Open-Source</li>
</ul>
</div>

<div class="right">
![](assets/images/galaxy/galaxy_interface.png)
https://galaxyproject.org
</div>

---

### The Galaxy Interface


![](assets/images/galaxy/galaxy_instance_detailed_screenshot.png)

---

### Bioinformaticsc: The Galaxy way

A `mothur` command in Galaxy:

<div class="left">
![](assets/images/microbiota/mothur_commandline.png)

</div>
<div class="right">
![](assets/images/galaxy/mothur_tool_interface.png)
</div>

---

### Analysis History

<div class="left small">
<ul>
<li> Examine datasets, add metadata </li><br>
<li> Galaxy houdt analyse historie exact bij</li>
  <ul>
  <li> Tools & versions</li>
  <li> Parameter settings</li>
  <li> Input and reference datasets</li>
  </ul><br>
<li> Colours indicate status </li>
  <ul>
  <li> <a style="background-color: gray; color: white;">Grey:</a> queued </li>
  <li> <a style="background-color: yellow; color: black;">Yellow:</a> running </li>
  <li> <a style="background-color: green; color: white;">Green:</a> completed successfully </li>
  <li> <a style="background-color: red; color: white;">Red:</a> error occurred </li>
  </ul><br>
<li> Download, run info, restart, visualisations </li>
</ul>
</div>
<div class="right">
![scale-30](assets/images/galaxy/history.png)
</div>

---

### Workflows

Tools are easily combined into analysis pipelines using the graphical *workflow editor*


![scale-80](assets/images/galaxy/workflow_editor.png)

---

### Workflows

Starting a workflow

![scale-70](2018-StreeklabHaarlem/images/hladq_workflow_run.png)

---

### Visualisations

<div class="small left">
<ul>
  <li> Built-in visualisation plug-ins and genome browser </li>
  <li> Connections to online visualisation providers </li>
  <li> Tools that produce visualisations </li>
</ul>
</div>
<div class="right">
![](assets/images/galaxy/visualisations.png)
</div>
---

### Share your work

<div class="small left">
<ul>
<li> Datasets, Histories, Workflows, Visualisations</li>
  <ul>
  <li>Specific users </li>
  <li>Anybody with the link</li>
  <li>Publicly visible </li>
  </ul>
</ul>
</div>
<div class="right">
![](assets/images/galaxy/shared_data.png)
</div>
---

### Galaxy Training

Central repository of Galaxy Training materials

![scale-50](assets/images/galaxy/training_materials_website.png)

https://training.galaxyproject.org


---

### Microbiota Analyses

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

![](assets/images/microbiota/human_microbiome.png)

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
![unbalanced scale-50](assets/images/microbiota/dysbiosis-balance.png)
![diseases](assets/images/microbiota/microbiota-disease.jpg)

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

![](assets/images/microbiota/slh-logo2.png)
![](assets/images/microbiota/slh-envelope.png)

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
![](assets/images/microbiota/slh-culture.jpg)
</div>

Note:
- MALDI: Matrix Assisted Laser Desorption/Ionization
- TOF MS: Time of Flight Mass spectrometry

- Bacteria grown on selective medium
 - Not all bacteria thrive equally (or at all) on medium
 - optimized to quickly show known pathogens
 - but "rest" can also be interesting
 - anaerobic bacteria are hard to grow in lab

- 16S cannot show antibiotic resistance, and only reliable down to genus level
- Time: 16S usually equally quick
 - 16S 2-3 days
 - cultures: mostly 24-48 hours, some types difficult to culture and can take 2 weeks

- Costs: NGS higher, but when culture is negative, cheaper than hospitalization

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

### Streeklab Haarlem


![scale-70](assets/images/microbiota/16S_end-to-end.png)
![scale-50](assets/images/microbiota/so_much_data.png)

---

### Galaxy!

![](assets/images/microbiota/workflow.png)

---


### Results reporting

---

### Krona

![scale-50](assets/images/microbiota/krona.png)

<div class="tiny">
doi: 10.1186/1471-2105-12-385
</div>
---

<embed src="https://marbl.github.io/Krona/examples/rdp.krona.html">

---

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
![](assets/images/microbiota/arthritis.png)
</div>


---

### Conclusions

<div class="small">
<ul>
 <li>Pipeline offers precise quantitative microbiota analyses</li>
 <li>Can offer insight where culture was negative</li>
 <li>Suitable for samples of low biomassa</li>
 <li>Clinicians can use pipeline without bioinformaticians help </li>
</ul>
</div>

---

### Run it in the SURF HPC Cloud?

<div class="small">
<ul>
 <li> Streeklab Haarlem does not have the expertise to run this in-house </li>
 <li> We don't have resources to support/maintain this </li>
 <li> Typically run the workflow ~once a week </li>
  <ul>
   <li>Spin up VM, run workflow, download results, shut down VM</li>
  </ul>
</ul>
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

