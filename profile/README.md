# AutoMech

AutoMech calculates high-level *ab initio* thermochemical and kinetic data for chemical kinetic models.

It consists of a hierarchy of five modules:

 - [MechDriver](https://github.com/Auto-Mech/mechdriver): Top-level workflow drivers
 - [MechAnalyzer](https://github.com/Auto-Mech/mechanalyzer): Mechanism pre- and post-processing
 - [AutoFile](https://github.com/Auto-Mech/autofile): Filesystem databasing
 - [AutoIO](https://github.com/Auto-Mech/autoio): I/O interfaces to external programs
 - [AutoChem](https://github.com/Auto-Mech/autochem): Cheminformatics and coordinate transformation


## Contribute

The AutoMech code is in development, so we encourage users to install it in developer mode (see below) and send us bug reports,
or submit pull requests they are comfortable.

## Install

To install the code in developer mode, fork and clone the [MechDriver](https://github.com/Auto-Mech/mechdriver) repository
and follow the instructions in its [README](https://github.com/Auto-Mech/mechdriver?tab=readme-ov-file#install).

~~End-users who do not wish to contribute can install the code using
[Conda](https://docs.anaconda.com/miniconda/#quick-command-line-install),
[Mamba](https://github.com/conda-forge/miniforge?tab=readme-ov-file#install), or
[Pixi](https://pixi.sh/latest/#installation).~~

## Use

To learn how to run the code, you can get started with the `quick` example
[here](https://github.com/Auto-Mech/mechdriver/tree/dev/examples) before moving on to more advanced examples.
To run the code, make sure you have the desired electronic structure packages in your path, then enter one of
the example directories and run the following command:
```
automech run &> out.log &
```

[^1]: For Conda/Mamba, you can add this channel using `conda config --append channels auto-mech`.
For Pixi, you can use `pixi project channel add auto-mech`.

[^2]: For Pixi, `conda-forge` is automatically the default channel. For Conda/Mamba, unless installed through
the Miniforge distribution, you will need to set this configuration using `conda config --prepend channels conda-forge`.

