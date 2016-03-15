# Exercices with GATE

This pages propose some exercices with the GATE software developed by the [Opengate](http://www.opengatecollaboration.org) collaboration. GATE allows to perform various Monte-Carlo simulations in medical physics.

Simulations are organized in a folder, with the following subfolders : ```data```, ```mac``` and ```output```. Macros files are stored in ```mac```. Gate *must* be run in the initial simulation folder, such as : ```Gate mac/main.mac``` (don't forget the ```mac/```). The macros that make use of data *must* refer to the ```data/``` subfolder.

Follow the following exercises and provide a written report. The general idea it to try to understand every commands in the macro files to be able to analyze the results.

Simulations macros may be found in this [zip](https://www.creatis.insa-lyon.fr/~dsarrut/dqprm/gate-simulations.zip).

Others documents:
- [Slides](https://www.creatis.insa-lyon.fr/~dsarrut/dqprm/simulation-dqprm-2016.pdf)
- Linux command line help: [Pocket guide](http://www.cheatography.com/kesavanbr/cheat-sheets/pocket-guide-linux-commands) or [Cmd line](http://www.cheatography.com/davechild/cheat-sheets/linux-command-line)
- Gate documentation can be found [here](http://wiki.opengatecollaboration.org/index.php/Users_Guide_V7.2)
- List of [radionuclides](http://www.nucleide.org/DDEP_WG/DDEPdata.htm)
- Page of image viewer [vv](http://vv.creatis.insa-lyon.fr)

To analyze simulations, you need additional software. For example:
- Nuclear physics toolkit [root](https://root.cern.ch)
- Simple and fast plot [gnuplot](http://www.gnuplot.info)
- Complete matlab like langage: [python](https://www.python.org) with scientific module: [scipy](http://www.scipy.org)

Question ? [david.sarrut@creatis.insa-lyon.fr](david.sarrut@creatis.insa-lyon.fr)


DQPRM 2016: add the following lines at the end of the file ```.bashrc```.

```
export LD_LIBRARY_PATH=/usr/local/clhep_2.1.1.0/lib/:$LD_LIBRARY_PATH
source /opt/root-5.34/bin/thisroot.sh
source /usr/local/geant4.10.2.p01-install/bin/geant4.sh
export PATH=${PATH}:/usr/local/geant4.10.2.p01-install/bin
export LD_LIBRARY_PATH=${LD_LIBRARY_PATH}:/usr/local/geant4.10.2.p01-install/lib64
export PATH=/usr/local/gate_v7.2-install/bin:$PATH
```




