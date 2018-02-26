# Exercise 7 (CBCT)

Now create a simulation from scratch: the goal is to simulate the acquisition of a x-ray cone-beam radiography. Create a world containing a patient ct image and a detector located about 50 cm away from the patient. Add a photon source emitting gamma of 60 keV energy, with a 8x8mm square and a divergent beam, pointing to the patient and the detector. Record the photon fluence on the detector by using a ```FluenceActor``` ([photon counting](http://wiki.opengatecollaboration.org/index.php/Users_Guide:Tools_to_Interact_with_the_Simulation_:_Actors#Fluence_Actor_.28particle_counting.29)). The goal is to produce two radiographies of the patient, at 0 and 90 degree.

![](/assets/simu-cbct.png)

