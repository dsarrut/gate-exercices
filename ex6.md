# Exercice 6

We now consider the simulation of internal radiation therapy treatment with an agent labelled with Yttrium 90. 90Y emits a continuous spectrum of electron with a mean energy aroun 927 keV and a maximum at 2.28 MeV. Several SPECT images have been merged together to produce a time-integrated activity emission map (TIA) associated with a patient CT. Create a simulation that uses this TIA as a voxelized source, see macro 'source-vox.mac'. The pixels in the TIA image are expressed in MBq.h. Create a simulation that compute the dose resulting from this activity map on the given patient image ('ct1-4mm.mhd'). Instead of 'setTotalNumberOfPrimaries', consider the following macro to set the simulation time :

```
 /gate/application/setTimeStart     0. s
 /gate/application/setTimeStop      1 s
 /gate/application/startDAQ
 ```

Perform a simulation with about 2 millionth of seconds. Analyze the results, and in particular the number of simulated particles.
