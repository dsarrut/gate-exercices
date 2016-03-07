# Exercice 1


### Step 1
 
Go into the folder 'cd exercices'. Read the file 'mac/ex1.mac'. Run the simulation 'Gate mac/ex1.mac' and analyze the results. Describe all the outputs. Display the curves (with gnuplot or matlab or excel or R ...). For example, to use gnuplot, go in the 'gp' folder, type 'gnuplot'. Then type 'load "plot-ex1.gp"'. Look the content of the file 'plot-ex1.gp' to understand how to generate a plot.

Back to Gate macros. You can play with the verbose options in the verbose.mac file and with the commands '/tracking/verbose'. For this later command, use 'Gate mac/ex1.mac | more' to display the terminal output page by page.

In most of the macro, you can enable visualization with two steps: 1) uncomment the line in the macro that include the file 'mac/visu.mac' and 2) execute Gate with the '-qt' option : 'Gate -qt mac/ex1.mac'. Be careful to reduce the number of primaries to a very low number (around 10 max) before launching the visualization.

### Step 2

Change the number of simulated particles (primaries Events). What are the changes regarding the results ? Comment the computing time, the uncertainties. Analyze a bit deeper the "gamma-stat.txt" file, what can you say about the Events/Tracks/Steps ? How to estimate the number of particles needed to reach 1% uncertainty in a given region of interest ?

### Step 3

Change the target (the phantom). Insert an aluminum box somewhere in the beam path, comment the results in term of dose, uncertainty, computing time, number of Track/Steps etc. Modify the production cuts and analyse the differences.

### Step 4

Modify the DoseActor. Change parameters : size, resolution, voxel size, position etc (but keep 1D measurements and .txt file format). Observe the results and comments.

