# LISETTA

LISETTA is a FairRoot-based software for the analysis of LISA + AGATA experimental data. 

Contact: calum.e.jones@gmail.com

Development:
* Calum Eoin Jones
* Elisa Maria Gandolfo


Requirements:
* ucesb, specifically: https://git.chalmers.se/expsubphys/ucesb.git
* FairSoft: https://github.com/FairRootGroup/FairSoft
* FairRoot: https://github.com/FairRootGroup/FairRoot
* cmake v13.3+

The latest prod version of both FairSoft and FairRoot can be found on the lx-pool GSI computers.

Before compiling, please make the empty UCESB unpacker! I.e.:

```
> cd ucesb
> make empty -j
> cd ..
```

To compile:
```
> export SIMPATH=/path/to/fairsoft
> export FAIRROOTPATH=/path/to/fairroot
> export UCESB_DIR=/path/to/ucesb
> git clone https://github.com/cej25/c4Root.git
> mkdir build
> cd build
> cmake ../c4Root
> . ./config.sh
> make -j
```

