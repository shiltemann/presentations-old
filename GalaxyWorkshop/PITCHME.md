# Let's get started!

<div class="bottom small">
(These slides can be accessed via: https://tinyurl.com/GalaxyWorkshop)
</div>

---

## Course Overview

<ul>
 <li>**Aim** provide you with the knowledge to use Galaxy for your daily analysis</li>
 <li>**Prosepective**</li>
 <ul>
  <li>The importance of bioinformatics in Research (Guido Jenster)</li>
  <li>FAIR data analysis and large informatics projects (Andrew Stubbs)</li>
  <li>Galaxy and Beyond (advanced topics and wider Galaxy ecosystem)(Saskia Hiltemann)</li>
 </ul>
 <li>**Objectives**</li>
 <ul>
  <li>DNA, RNA, microbiome all influence our health</li>
  <ul>
   <li>Familiarize yourself with the Galaxy interface by performing simple DNA-seq analysis</li>
   <li>RNA-seq end-to-end analysis (QC, mapping, DEA, visualisation)</li>
   <li>16S rRNA seq bacterial analysis </li>
  </ul>
  <li>Set up a working community within EMc (and outside) for Galaxy questions</li>
 </ul>
</ul>


---

## Programme: Day 1


| Tables   |      Are      |  Cool |
|----------|:-------------:|------:|
| col 1 is |  left-aligned | $1600 |
| col 2 is |    centered   |   $12 |
| col 3 is | right-aligned |    $1 |

--



## Organizational remarks

+++

<div class="left">
<br><br>
<ul>
 <li>Please fill out the sign-in sheet </li>
 <br>
 <li> Star
 <li> Coffee will 11:00 and 15:30 </li>
 <li> Lunch will be at 13:00 </li>
</ul>
</div>

<div class="right">

![scale-70](assets/images/workshop/signin.png)
<br>
![scale-20](assets/images/workshop/hotdrink.jpg)
![scale-20](assets/images/workshop/food.gif)
![scale-20](assets/images/workshop/drinks.jpeg)


</div>

---

## Programme


---

## Introduce yourself

(You don't have to follow this:)

<div class="left">
  <br>
  <ul>
    <li> Who are you? </li>
    <li> Where are you from? </li>
    <li> What do you do? </li>
    <li> Why do you join the workshop? </li>
  </ul>
</div>

---

## Sticky Notes

---

## Sticky Notes

<div class="small left70">
<br><br><br>
<ol>
  <li> Status indicators
  <ul>
   <li> Pink: Put on screen when you have a question</li>
   <li> Green: Used to indicate your progress</li>
  </ul>
  </li>
  <br>
 <li>  End-of-day feedback
  <ul>
   <li> Green: What did you like?</li>
   <li> Pink: What could we improve tomorrow? </li>
   <li> Leave on blackboard at end of the day </li>
  </ul>
 </li>
</ol>
</div>

<div class="right30">
![scale](assets/images/workshop/stickynotes.jpeg)

![scale](assets/images/workshop/stickynotes_feedback.png)
</div>

---

# Day 1

+++

## Galaxy

1. Open Galaxy: https://usegalaxy.eu

2. Register for an account (top right)

3. Verify your registration (e-mail confirmation)

3. Join the workshop: https://usegalaxy.eu/join-training/ElixirNL2018


+++

### Training manual (Morning)

1. Navigate to: https://training.galaxyproject.org

2. Choose topic: **Introduction to Galaxy Analyses**

3. Choose tutorial: **From Peaks to Genes**

4. Have fun!

5. Submit feedback form at end of tutorial


+++

## Wrap-up

1. Questions?

2. Please fill in the feedback form to help us improve the tutorial!

3. Thank you for participating!


+++

### Training manual (Afternoon)

1. Navigate to: https://training.galaxyproject.org

2. Choose topic: **Transcriptomics**

3. Choose tutorial: **Reference-based RNA-Seq data analysis**

4. Have fun!

5. Submit geedback form at end of tutorial

+++

## Wrap-up

1. Questions?

2. Please fill in the feedback form to help us improve the tutorial!

3. Thank you for participating!

4. Leave your sticky notes with feedback to help us improve the course!

---

# Day 2

+++

### Training manual (Morning Day 2)

1. Navigate to: https://training.galaxyproject.org

2. Choose topic: **Transcriptomics**

3. Choose tutorial: **Pinpoint key pathways using Heinz**

4. Have fun!

5. Submit feedback form at end of tutorial

+++

## Wrap-up

1. Questions?

2. Please fill in the feedback form to help us improve the tutorial!

3. Thank you for participating!


+++

### Training manual (Afternoon)

1. Navigate to: https://training.galaxyproject.org

2. Choose topic: **Metagenomics**

3. Choose tutorial: **16S Microbial Analysis with Mothur**

4. Have fun!

5. Submit feedback form at end of tutorial

+++

## Wrap-up

1. Questions?

2. Please fill in the feedback form to help us improve the tutorial!

3. Thank you for participating!

4. Leave your sticky notes with feedback to help us improve the course!

---

# Day 3

+++

### Computer room

<div class="left">
<ul>

<li> Log in to a Linux computer </li>
  <pre>
  Username: Wshop01
  Password: Friday19!</pre>
<li> We will be using the following software: </li>
 <ul>
  <li>`Terminal`</li>
  <li>`Firefox`</li>
  <li>`Files`</li>
  <li>`Text Editor`</li>
 </ul>
</ul>
</div>

<div class="right">
![](assets/images/workshop/a-list-of-software.png)
</div>

+++

### Set up Cloud VM

<div class="small">
<ol>
<li>Get a Cloud VM IP by signing in https://course.page.link/gcloud </li>
<br>
<li>Download the login key 'galaxy-2018' from https://course.page.link/key via Firefox</li>
  <ul>
  <li>The path to key file is `~/Downloads/galaxy-2018` or wherever </li>
  <li>Change the permission: `chown 700 ~/Downloads/galaxy-2018`</li>
 </ul>
<br>
<li>Save these lines below into a file named 'config' in `~/.ssh/` </li>
  <ul>
   <li> Replace IP with the one you just got.</li>
   <li> Change the permission `chown 600 ~/.ssh/config` </li>
  </ul>
<pre>
host galaxy
     HostName IP
     IdentityFile ~/Downloads/galaxy-2018
     User ubuntu
</pre>
<br>
<li> Set up sftp mount </li>
 <ul>
  <li> Open 'Files', click '+ Other Locations' </li>
  <li> type `ssh://galaxy/home/ubuntu` (on the right of **Connect to Server**) and press 'Enter'</li>
 </ul>
</ul>



</div>

+++


### Work with Cloud VM

- Log in to the cloud VM via this command:
  <pre>ssh -L 4000:localhost:4000 galaxy</pre>
- Build the training website
  <pre>
   cd ~/training-material/
   make serve
  </pre>
- Open Firefox, and go to
  http://localhost:4000/training-material/

+++

### Edit a file in the Cloud VM

<div class="small alignleft">

Here is just an example, you can modify other files as you wish.

<br><br>

<ol>
 <li> Open 'Files', click 'galaxy' on the left (the navigation panel) </li>
 <li> Open `training-material/topics/metagenomics/tutorials/mothur-miseq-sop/tutorial.md` <br> with `Text Editor` </li>
 <li> Make any change you want and save. </li>
 <li> View the change by the link in Firefox </li>
   <ul>
    <li> http://localhost:4000/training-material/ </li>
    <li> topic: metagenomics </li>
    <li> tutorial: 16S rRNA sequencing with mothur </li>
   </ul>
</ol>

</div>

+++

### Training manual (Afternoon)

1. Navigate to: https://training.galaxyproject.org

2. Choose topic: **Contributing to the Galaxy Training Material**

3. We will be doing multiple tutorials

4. Have fun!

5. Submit feedback form at end of tutorial

+++

## Wrap-up

1. Questions?

2. Please fill in the feedback form to help us improve the tutorial!

3. Thank you for participating!

4. Leave your sticky notes with feedback to help us improve the course!


---

## Final wrap-up

Thank all the lecturers, speakers and helpers for their efforts into this training course.

+++

## Final wrap-up

<div class="left">
 <br>
 <ul>
  <li> Please return your badges </li>
  <br>
  <li> Please fill in the feedback form </li>
  <br>
  <li> Thank you for joining! </li>
 </ul>
</div>
<div class="right">
![scale-40](assets/images/workshop/badges.png)
![scale-70](assets/images/workshop/feedback.jpg)
</div>
