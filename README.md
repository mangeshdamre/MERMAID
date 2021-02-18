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

## Coarse-grained molecular dynamics parameters
In MERMAID web server, Coarse-grained simulation will be performed in four stages namely
1. Minimization;
2. Equilibration at constant volume (NVT);
3. Equilibration at constant pressure (NPT); and
4. Production.

### Set minimization parameters
The user will see the default minimization parameters to perform the minimization of the Coarse-grained system. User can modify the parameters as per the experimental requirments. The molecular dynamics parameters such as 'integrator, tinit, dt, nsteps, init-step, comm-mode, nstcomm, comm-grps' etc. are well explained and the user can get detailed information about parameters in the **<a href="http://manual.gromacs.org/archive/4.6.3/online/mdp_opt.html" target="_blank">Gromacs MDP</a>** page.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter8.png" width="225" />
</p>

### Set Equilibration (NVT) parameters
The user will see the default equilibration parameters (at constant volume) to perform the equilibration of the coarse grained system. The user can modify the parameters as per the experimental requirements.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter9.png" width="225" />
</p>

### Set Equilibration (NPT) parameters
The user will see the default equilibration parameters (at constant pressure) to perform the equilibration of the coarse grained system. User can modify the parameters as per the experimental requirements.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter10.png" width="225" />
</p>

### Set Production parameters
The user will see the default production parameters to perform the molecular dynamics simulation of the Coarse-grained system. User can modify the parameters as per the experimental requirements.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter11.png" width="225" />
</p>
After modifying all the parameters as per experimental requirment user need to submit these parameters by clicking on <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/tab4.png" width="100" /> tab. After submitting the parameters, user will be redirect to the new page displaying Welcome message with the link to bookmark the link to the result page.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter12.png" width="225" />
</p>

## MERMAID Results
The Bookmark link will redirect the user to MERMAID result page in which the user will have access to all the generated input and output files.

### MERMAID output files
The user can see the input and output files generated by MERMAID server. All the files can be download by clicking the link <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/tab2.png" width="250" />. User can extract the files to the local system and can perform the analysis.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter13.png" width="225" />
</p>

### MERMAID output structure visualization
The user can visualize the atomistic structure of membrane protein in the browser. The user can also see the initial coarse-grained system structure, the structure of minimized system, the structure of the equilibrated system at constant volume, the structure of the equilibrated system at constant volume and finally the structure produced in production phase.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter14.png" width="225" />
</p>

## MERMAID simulation analysis
After a successfull completion of membrane protein coarse-grained simulation, the user can visualize some basic analysis performed by MERMAID web server.

### Coarse-grained analysis
The user can click on the tab <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/tab1.png" width="225" />. It will redirect the user to the analysis page where user can see the multiple charts.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/parameter13_1.png" width="225" />
</p>
It will redirect the user to the analysis page in which is possible seeing multiple charts. Furthermore, the user can analyze different properties of the coarse-grained system like system stability during minimization of the coarse-grained system. Also, the user can see the analysis performed on production phase for different properties: potential energy, kinetic energy, total energy, the temperature of the system, the pressure of the system, the volume of the system, the density of the system, and enthalpy of the system, etc. All the charts are very interactive in nature. The user can download all the charts.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/chart2.png" width="225" />
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/chart1.png" width="225" />
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/chart3.png" width="225" />
</p>

## Run MERMAID system on local system
The main advantage of MERMAID web server is that it not only provide the possibility to run the simulation but also allow the user to download the files to run the coarse-graine simulations on users local system.

### Run MERMAID locally
The user can download the initial files to run the coarse-grained simulation locally. First, the user need to click on <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/tab3.png" width="225" /> tab.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/inputs.png" width="225" />
</p>
It will download the MERMAID_DIR.tar file. Extract all the content of the tar file in a folder.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/search3.png" width="225" />
</p>
In the extracted folder, the user will see shell script file MERMAID_simulation_run.sh. The user should open the shell script file and follow the instructions given inside to perform coarsed-grained simulation locally.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/scriptrun.png" width="225" />
</p>

## Search your simulation
The user can search for their completed projects in MERMAID web server by using search function.

### Search function
The user can use the search function to search their project. It will redirect to the respective project where user can check all their simulation jobs.
Further the user can follow the steps from point **10 to 13**.
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/search1.png" width="500" />
</p>
<p float="center">
  <img src="https://github.com/mangeshdamre/MERMAID/blob/main/Images/search3.png" width="225" />
</p>

## Video Tutorial
The user can take a look in video tutorial which demonstrate the use of MERMAID web server.
[Click here to follow MERMAID video tutorials!](https://www.youtube.com/watch?v=hbwI7YnonEY)

### How to cite this work?
MERMAID: dedicated web server to prepare and run coarse-grained membrane protein dynamics
Nucleic Acids Research, Volume 47, Issue W1, 02 July 2019, Pages W456–W461, 
https://doi.org/10.1093/nar/gkz416

BIBTEX
`
@article{damre2019mermaid,
  title={MERMAID: dedicated web server to prepare and run coarse-grained membrane protein dynamics},
  author={Damre, Mangesh and Marchetto, Alessandro and Giorgetti, Alejandro},
  journal={Nucleic acids research},
  volume={47},
  number={W1},
  pages={W456--W461},
  year={2019},
  publisher={Oxford University Press}
}
`
