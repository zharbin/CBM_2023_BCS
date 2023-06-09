# CBM_2023_BCS
Healing Following BCS Finite Element Code

Publication:
#### Computational Mechanobiology Model Evaluating Healing of Postoperative Cavities Following Breast-Conserving Surgery
#### Zachary Harbin, David Sohutskay, Emma Vanderlaan, Muira Fontaine, Carly Mendenhall, Carla Fisher, Sherry Voytik-Harbin, Adrian Buganza Tepole

The code has been designed to run on Purdue Research Computing Clusters. It may not work as-is in your system. Here are a few tips to troubleshoot compiling:
<ul>
<li>The code requires EIGEN linear algebra libraries, as well as BOOST libraries. It currently runs witn BOOST 1.75 and EIGEN 3.2.10</li>
<li>The code has a parallel version with OPEN MP. The parallel parts of the code are primarily in solver.cpp and can be easily commented out if desired</li>
<li>Compilation is done with CMAKE</li>
</ul>

To compile the code:
<ul>
<li>Make sure EIGEN and BOOST files are downloaded in the folder in which the folder CBM_2023_BCS is located</li>
<li>Open terminal. Make sure CMAKE is installed, as well as C++ compilers. We use intel compilers with support for OPEN MP.</li>
<li>Go to the folder where the code will be compiled (i.e., cmake-build-release)</li>
<li>Run CMAKE in the terminal to create the makefile (i.e., cmake ../   make/)</li>
<li>The code can then be executed through the following command: sbatch surgerywoundcpp3D.sub</li>
</ul>
