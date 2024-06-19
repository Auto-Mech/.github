# AutoMech

AutoMech calculates high-level *ab initio* thermochemical and kinetic data for chemical kinetic models.

It consists of a hierarchy of five modules:

 - [MechDriver](https://github.com/Auto-Mech/mechdriver): Top-level workflow drivers
 - [MechAnalyzer](https://github.com/Auto-Mech/mechanalyzer): Mechanism pre- and post-processing
 - [AutoFile](https://github.com/Auto-Mech/autofile): Filesystem databasing
 - [AutoIO](https://github.com/Auto-Mech/autoio): I/O interfaces to external programs
 - [AutoChem](https://github.com/Auto-Mech/autochem): Cheminformatics and coordinate transformation


## Contribute

The AutoMech code is in development, so we encourage users to install it in developer mode and send us bug reports.
See
[here](https://github.com/avcopan/amech-dev?tab=readme-ov-file#automech-developer-set-up)
for instructions to get set up.


## Install

End-users who are unable to contribute (see above) can install the code using Conda, Mamba, or Pixi.
```
conda install automech # option 1
mamba install automech # option 2
pixi add automech      # option 3
```
Before running the above command, you will need to add `auto-mech` to your list of
channels:
```
conda config --append channels auto-mech # option 1 and 2
pixi project channel add auto-mech       # option 3
```
If `conda-forge` isn't the default channel for your Conda/Mamba installation, you will
also need to set this additional configuration using the command above with `--prepend`.

