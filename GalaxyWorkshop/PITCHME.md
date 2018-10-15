# Let's get started!

Note:

These slides can be accessed via: https://tinyurl.com/GalaxyWorkshop

---

## Organizational remarks

+++

<div class="left">
<br><br>
<ul>
 <li>Please fill out the sign-in sheet </li>
 <br>
 <li> Coffee will be at each session break  </li>
 <li> Lunch will be at 13:00 </li>
 <li> Drinks will be at 17:00 </li>
 <li> A complete schedule is in https://galaxy-2018.bioinformatician.science/program</li>
</ul>
</div>

<div class="right">

![scale-70](assets/images/workshop/signin.png)
<br>
![scale-20](assets/images/workshop/hotdrink.jpg)
![scale-20](assets/images/workshop/food.gif)
![scale-20](assets/images/workshop/drinks.jpeg)


</div>

+++

## Social dinner

<div class="left">
 <br>
 <ul>
  <li> **Time:** Thursday, 19:00 </li>
  <li> **Restaurant:** 1e Klas </li>
  <li> **Location:** Amsterdam CS </li>
  <li> **Getting there:** </li>
 </ul>
</div>

<div class="right">

![](https://restaurant1eklas.nl/wp-content/uploads/2015/07/Amdsterdam-Central-Station-Amsterdam-January-2012-Alexander-T-2000x1333.jpg)

![](https://www.restaurant1eklas.nl/wp-content/uploads/2016/09/1D3B2191-e1473928938346.jpg)

</div>

+++

## Introduce yourself

You don't have to follow this:
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

<div class="small left70">
<br><br><br>
<ol>
  <li> Status indicators
  <ul>
   <li>Pink: put on screen when you have a question</li>
   <li>Green: used to indicate your progress</li>
  </ul>
  </li>
  <br>
 <li>  End-of-day feedback
  <ul>
   <li> Green: what did you like?</li>
   <li> Pink: what could we improve tomorrow? </li>
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

5. Submit feedback form at end of tutorial if you have comments/suggestions


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

5. Submit feedback form at end of tutorial if you have comments/suggestions

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

5. Submit feedback form at end of tutorial if you have comments/suggestions

+++

## Wrap-up

1. Questions?

2. Please fill in the feedback form to help us improve the tutorial!

3. Thank you for participating!


+++

### Training manual (Afternoon Day 2)

1. Navigate to: https://training.galaxyproject.org

2. Choose topic: **Metagenomics**

3. Choose tutorial: **16S Microbial Analysis with Mothur**

4. Have fun!

5. Submit feedback form at end of tutorial if you have comments/suggestions

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

- Log in to computer with a ticket you received from the lecturers.
- Get a Cloud VM IP by signing in ...
- Download the login key 'galaxy-2018' from https://course.page.link/key via Firefox
  - The path to key file is `~/Downloads/galaxy-2018` or something else you should know
  - Change the permission: `chown 700 ~/Downloads/galaxy-2018`
- Save these lines into a file named 'config' in `~/.ssh/`
```
host galaxy
     HostName IP
     IdentityFile ~/Downloads/galaxy-2018
     User ubuntu
```
  - Replace IP with the one you just got.
  - Change the permission chown 600 ~/.ssh/config
- Set up sftp mount
  - Open 'Files', click '+ Other Locations'
  - type `ssh://galaxy/home/ubuntu`


+++


### Cloud VMs

- Log in to the cloud VM via this command: `ssh -L 4000:localhost:4000 galaxy`
- Go to ... `make serve`
- Open Firefox, type `http://localhost:4000`

+++

### Training manual (Afternoon Day 3)

1. Navigate to: https://training.galaxyproject.org

2. Choose topic: **Metagenomics**

3. Choose tutorial: **16S Microbial Analysis with Mothur**

4. Have fun!

5. Submit feedback form at end of tutorial if you have comments/suggestions

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
