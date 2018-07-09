# Exercise1 - start

## Step 1

Go into the folder `cd exercices`. Read carefully the file `mac/ex1.mac` to understand what is the purpose of the simulation. Note: the command `/control/execute <filename>` includes the content of the give file. This command allows to split simulation macros in several files.

Run the simulation with `Gate mac/ex1.mac` and analyze the results. Describe all the outputs. Display the curves \(with python or gnuplot or matlab or excel or R ...\). For example, you can plot the curve with python by typing `./py/plot.py` from the folder `exercices`. Look at the file `./py/plot.py`, it use python code to load the output file of the simulation and create curves. Python is a powerful language for data analysis. You may want to investigate it from the [main web site](https://docs.python.org/3/tutorial/index.html). The two Python packages that are useful for us here are: [numpy](http://www.numpy.org/) \(for scientific calculation\) and [matplotlib](https://matplotlib.org/) for plotting.

Back to Gate macros. You can play with the verbose options in the verbose.mac file and with the commands: `/tracking/verbose 2` \(change the number to increase the verbosity\).

For this later command, use `Gate mac/ex1.mac | more` to display the terminal output page by page. Warning, using verbose may increase the computation time, you should only use large verbose value for debug purpose not for production. You may also use `Gate mac/ex1.mac > result.txt` it will create a file named `result.txt` that will contains all text written on the screen by Gate.

In most of the macro, you can enable visualization with two steps: 1\) uncomment the line in the macro that include the file `mac/visu.mac` and 2\) execute Gate with the `--qt` option : `Gate --qt mac/ex1.mac`. Be careful to reduce the number of primaries to a very low number \(around 10 max\) before launching the visualization.

## Step 2

Change the number of simulated particles \(primaries Events\). What are the changes regarding the results? Comment the computing time, the uncertainties. Analyze a bit deeper the `gamma-stat.txt` file, what can be said about the Events/Tracks/Steps ? How to estimate the number of particles needed to reach 1% uncertainty in a given region of interest ?

## Step 3

Change the target \(the phantom\). Insert for example an aluminum box somewhere in the beam path, comment the results in term of dose, uncertainty, computing time, number of Track/Steps etc. Modify the production cuts and analyse the differences.

## Step 4

Modify the `DoseActor`. Change parameters: size, resolution, voxel size, position etc \(but keep 1D measurements and .txt file format\). Observe the results and comments.

## Step 5

Got the the python notebook to start interactive analysis : [http://localhost:8889/notebooks/exercice%20dose%20depth%20profile.ipynb](http://localhost:8889/notebooks/exercice%20dose%20depth%20profile.ipynb)



