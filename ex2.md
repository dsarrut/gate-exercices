# Exercice 2

Change for 3D dose distribution as described in ```ex2.mac```. Describe all the outputs. Analyse the 3D distribution (with ```vv```) and the 3D uncertainty. Analyse the ```stat-pat.txt``` file (with gnuplot file ```plot-ex2.gp```). Change the parameters of the 3D dose actor. Comments.

Example of command for vv : ```vv data/patient-2mm.mhd --fusion output/3d-pat-Edep.mhd``` to superimpose the computed edep to the CT image.

### Notes on coordinates systems



Gate/G4 manages its own coordinate system (world center)
Origin of the image is not used to position the image, position is, like all other volumes, according to the geometrical center of the image
However, two features are available:
“TranslateTheImageAtThisIsoCenter” allows to translate an image according to a coordinate given in the image coordinate system (thus taking origin into account)


 
