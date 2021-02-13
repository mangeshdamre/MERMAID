# MERMAID
https://molsim.sci.univr.it/mangesh/index.php

This tutorial introduces Coarse-grained simulation of membrane protein in presence of different concentrations of membrane lipids. The systematic workflow in this server is used to prepare initial coarse-grained system to run CG simulations. The MERMAID web server is used not only to run CG simulation but also it helps to generate the input files that can be downloaded at any moment of time to run locally by user. At the end of the tutorial, the user can also analyze the coarse-grained simulation trajectories. Let us go through MERMAID web server step by step. Detailed MERMAID workflow can be found **<a href="https://github.com/mangeshdamre/MERMAID/blob/main/Images/Detailed-workflow.jpg" target="_blank">here</a>**.

## System preparation

### Submit membrane protein structure
The prepation of Martini coarse-grained system is very easy with the help of MERMAID web server. User should write the project name in the given area which will be used in future to search the finished CGMD simulation. User have three possibilities to submit protein structure. The users can either upload their own membrane protein structure or can write the PDB ID in the given area which will retrive the protein structure either from **<a href="https://www.rcsb.org/structure/4UC1" target="_blank">RCSB</a>**  database or from **<a href="https://opm.phar.umich.edu/proteins/2750" target="_blank">OPM</a>**  database to the MERMAID server. On submission of protein structure to MERMAID, user will be redirect to molecular dynamics parameter page.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/uploadpdb1.png" width="225" />
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/uploadpdb2.png" width="225" /> 
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/uploadpdb3.png" width="225" />
</p>

### Molecular dynamics parameters (mdp)
After protein structure submission to MERMAID server, the user will have the access to the parameter page. Initially, the user can choose membrane concentration. MERMAID will give two possibilities to the user to select the membrane composition and their concentrations. MERMAID provides two types of Martini Forcefields (martini22 and martini22p).
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter1.png" width="225" />
</p>

### Membrane selection
In the <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/tab5.png" width="100" /> tab user will have access to already known membrane compostions. For example the user can chose the membrane compostion from any of the following-- 1] Plasma Membrane - human erythrocytes; 2] Plasma membrane - Rat Liver; 3] Endoplasmic Reticulum; 4] Golgi; 5] Lysosome; 6] Nuclear Membrane; 7] Mithocondria; 8] Neurons; 9] Myelin.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter4.png" width="225" />
</p>

In the <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/tab6.png" width="100" /> tab the user can change the concentraion of individual lipid present in the membrane as per experimental requirments.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter5.png" width="225" />
</p>

### Water selection and Box dimension
Further user can select the type of water and set the coarse-grained system dimensions.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter6.png" width="225" />
</p>

### Orientation of protein in the membrane
For membrane proteins, it is important to insert them properly inside the membrane. The user can have the freedom to align the protein inside the membrane or can keep the protein orientation as it is. Best practice is to check the already aligned membrane protein structure in **<a href="https://opm.phar.umich.edu/" target="_blank">OPM</a>** database and download the aligned structure. Submit the obtained structure from OPM server to the MERMAID server. For more details please check the section **"How to align membrane proteins?"** in **<a href="https://molsim.sci.univr.it/mangesh/questions.html#collapseThirteen" target="_blank">Q&A</a>** page.
