# AutoMech

AutoMech calculates high-level *ab initio* thermochemical and kinetic data for chemical kinetic models.

It consists of a hierarchy of five modules:

 - [MechDriver](https://github.com/Auto-Mech/mechdriver): Top-level workflow drivers
 - [MechAnalyzer](https://github.com/Auto-Mech/mechanalyzer): Mechanism pre- and post-processing
 - [AutoFile](https://github.com/Auto-Mech/autofile): Filesystem databasing
 - [AutoIO](https://github.com/Auto-Mech/autoio): I/O interfaces to external programs
 - [AutoChem](https://github.com/Auto-Mech/autochem): Cheminformatics and coordinate transformation


## Contribute

The AutoMech code is in development, so we encourage users to install it in developer mode and send us bug reports,
or even submit pull requests they are comfortable.
To install the code in developer mode, clone the [amech-dev](https://github.com/avcopan/amech-dev) repository
and follow the instructions in the [README](https://github.com/avcopan/amech-dev?tab=readme-ov-file#automech-developer-set-up)
to get set up.


## Install

End-users who do not wish to contribute can install the code using Conda, Mamba, or Pixi.
After adding `auto-mech` to your channels[^1] and making sure that `conda-forge` is your default channel,[^2]
the code can be installed as follows:
```
conda install automech # option 1
mamba install automech # option 2
pixi add automech      # option 3
```

## Use

To learn how to run the code, you can get started with the `simple` example
[here](https://github.com/Auto-Mech/mechdriver/tree/dev/examples) before moving on to more advanced examples.
To run the code, make sure you have the desired electronic structure packages in your path, then enter one of
the example directories and run the following command:
```
automech run &> out.log &
```

[^1]: For Conda/Mamba, you can add this channel using `conda config --append channels auto-mech`.
For Pixi, you can use `pixi project channel add auto-mech`.

[^2]: For Pixi, `conda-forge` is automatically the default channel. For Conda/Mamba, you may need
to set this configuration using `conda config --prepend channels conda-forge`.

