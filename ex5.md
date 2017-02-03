# Exercise 5 (TLE)


### Step 1

Go into the folder ```tle```. This simulation ```Gate mac/main.mac``` computes the dose deposition of a low energy x-ray irradiation (for example a during a radiography).

Dose convergence is very slow with conventional method. An additional actor is used named TLE for Track Length Estimator which is a VRT method proposed in the 80' (Williamson 87) allowing a much faster convergence (see for example the analysis in the article [[Baldacci2014]](https://www.creatis.insa-lyon.fr/site7/en/publications/BALD-15)). Compare the outputs ```dose-Dose.mhd``` and ``` dose-tle-Dose.mhd```, comment the differences. 

Gate output the Dose in Gy unit. Because very small number of particle is used, dose pixel values are around 10e-14 and so not easy to visualise: use the root macro file to normalise the dose map (normalise to the maximum value), type ```root -x normalise.C``` in the tle folder. Then the VV software can be used to visualize the dose distribution. Type ```vv data/phantom.mhd --fusion output/dose-tle-Dose.mhd data/phantom.mhd --fusion output/dose-Dose.mhd --linkall &``` to compare the dose maps. You can obtain help in VV by pressing F1.

### Step 2

Replace the 3D dose actor with a 1D dose depth profile (and associated uncertainty). Plot the depth dose with gnuplot for both conventional dose and TLE dose.

### Step 3

An improvement of the TLE method has been recently proposed. This method is named seTLE and include splitting. Execute and comment the macro ```main-setle.max``` that uses this seTLE method (described in [[Smekens2014]](https://www.creatis.insa-lyon.fr/site7/en/publications/SMEK-14)). Compare the number of simulated particle per second (PPS in the stat file), compare the dose convergence and the uncertainty.
