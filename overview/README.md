# Overview

In Gate, simulations are organized in a folder, with the following subfolders : `data`, `mac` and `output`. Macros files are stored in `mac`. Gate _must_ be run in the initial simulation folder, such as : `Gate mac/main.mac` \(don't forget the `mac/`\). The macros that make use of data _must_ refer to the `data/` subfolder.

The **source code** for the exercices below are in the folder `simulations/`

To start the  **analysis** with python notebook: 

* Go in the folder `simulations/ipynb`
* Start notebook server with: `jupyter notebook`
* Connect you browser to: [http://localhost:8889/tree](http://localhost:8889/tree) 

## Exercices about dose

* Exercice 1: photon beam, dose in water, 2D
* Exercice 2: photon beam, 3D dose map in 3D CT image
* Exercice 3: proton beam
* Exercice 4: simulation of a LINAC, phase-space concept
* Exercice 5: internal radiation therapy \(dosimetry\)

## Exercices about imaging

* Exercice 6: SPECT imaging
* Exercice 7: PET imaging

## Exercices about Variance Reduction Techniques \(VRT\)

* Exercice 8: Track Length Estimator, dose for low energy photon \(&lt;1 MeV\)
* Exercice 9: ConeBeam CT imaging with Fixed Forced Detection technique



