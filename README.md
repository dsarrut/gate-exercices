# Exercises with GATE

This pages propose some exercises with the GATE software developed by the [Opengate](http://www.opengatecollaboration.org) collaboration. GATE allows to perform various Monte-Carlo simulations in medical physics.

Simulations are organized in a folder, with the following subfolders : `data`, `mac` and `output`. Macros files are stored in `mac`. Gate _must_ be run in the initial simulation folder, such as : `Gate mac/main.mac` \(don't forget the `mac/`\). The macros that make use of data _must_ refer to the `data/` subfolder.

Follow the following exercises and provide a written report. The general idea it to try to understand every commands in the macro files to be able to analyze the results. Simulations macros may be found in this [zip](https://gitlab.in2p3.fr/david.sarrut/gate-exercices/repository/archive.zip?ref=1.0). 

For advanced user, the complete source code is available as a [git repository](https://gitlab.in2p3.fr/david.sarrut/gate-exercices). Required git-lfs. 

Others documents:

* Click [here for a pdf](https://www.gitbook.com/download/pdf/book/dsarrut/gate-exercises) version of this ebook
* [Slides](https://gitlab.in2p3.fr/david.sarrut/gate-exercices/blob/b7383664e69deca32db7b5e8cd3bfa9c4d1e7cdc/slides/simulation-dqprm-2016.pdf)
* Linux command line help: [Pocket guide](http://www.cheatography.com/kesavanbr/cheat-sheets/pocket-guide-linux-commands) or [Cmd line](http://www.cheatography.com/davechild/cheat-sheets/linux-command-line)
* Gate documentation can be found [here](http://wiki.opengatecollaboration.org/index.php/Users_Guide_V7.2)
* List of [radionuclides](http://www.nucleide.org/DDEP_WG/DDEPdata.htm)
* Page of image viewer [vv](http://vv.creatis.insa-lyon.fr)

To analyze simulations, you need additional software. For example:

* Nuclear physics toolkit [root](https://root.cern.ch)
* Simple and fast plot [gnuplot](http://www.gnuplot.info)
* Complete matlab like langage: [python](https://www.python.org) with scientific module: [scipy](http://www.scipy.org)

Question ? [david.sarrut@creatis.insa-lyon.fr](david.sarrut@creatis.insa-lyon.fr)

Source codes:

* Browse the code of the [exercices](https://gitlab.in2p3.fr/david.sarrut/gate-exercices/tree/master)
* GATE : [https://github.com/OpenGATE/Gate](https://github.com/OpenGATE/Gate)
* GateContrib: examples of simulations [https://github.com/OpenGATE/Gate](https://github.com/OpenGATE/GateContrib)
* Geant4: [http://geant4.cern.ch/support/download.shtml](http://geant4.cern.ch/support/download.shtml) 

&lt;!---  
**DQPRM 2016**

Add the following lines at the end of the file `.bashrc`.

```
source /opt/root-5.34/bin/thisroot.sh
source /usr/local/simu/geant4.10.02.p01-install/bin/geant4.sh
export PATH=${PATH}:/usr/local/simu/geant4.10.2.p01-install/bin
export LD_LIBRARY_PATH=${LD_LIBRARY_PATH}:/opt/qt5/5.2.0/gcc_64/lib/:/usr/local/simu/geant4.10.2.p01-install/lib64
export PATH=/usr/local/simu/Gate-v7.2-install/bin:$PATH
```

--&gt;

