# robotology-conda-binary-repackaging-recipes

Recipes for packaging as conda package closed source dependencies of robotology software, that are distributed in the `robotology` anaconda channel.
It is not where the conda recipes for robotology packages are either stored in conda-forge, or generated on the fly by the robotology-superbuild, see https://github.com/robotology/robotology-superbuild/blob/master/doc/conda-recipe-generation.md and https://github.com/robotology/robotology-superbuild/blob/master/doc/developers-faqs.md#how-to-ensure-that-binary-packages-are-correctly-generated-for-a-new-package for more info.


## How to install generated packages

To install the package generated by this repo, just use `conda` and specify that you want to install packages from the `robotology` channel.

To install the `esdcan` package:
~~~
conda install -c conda-forge -c robotology esdcan
~~~

To install the `ensenso` package:
~~~
conda install -c conda-forge -c robotology ensenso
~~~

At the moment, all packages are only available on Windows.

## How to regenerate packages and upload them on robotology (for developer, advanced)

If you modified the recipes contained in this repo (for example if you updated the version of the dependencies) and you want to regenerate and upload the conda packages, just run the `generate-conda-packages` GitHub Action Workflow. 

## Maintainers

This repository is maintained by:

| | |
|:---:|:---:|
| [<img src="https://github.com/traversaro.png" width="40">](https://github.com/traversaro) | [@traversaro](https://github.com/traversaro) 
