# Conda Cheatsheet
## Basic Conda 
###### Start conda:
`conda init`
###### Update conda:
`conda update conda`

## Environments
###### Create new environment with given Python version:
`conda create -n environmentName python=3.6`

###### Activate given environment:

`conda activate environmentName`

Deactivate given environment:

`conda deactivate`

###### List all Conda environments:

`conda env list`

###### Remove an environment:
(The environment must be inactive!)

`conda env remove --name environmentName`

## Packages
###### List all packages and versions in active environment:

`conda list`

###### Search a package to check if it is possible to install:

`conda search packageName`

###### Install a package in a given environment:

`conda install -n environmentName packageName`

###### Install a package in the active environment:

`conda install packageName`

###### Update a package in the active environment:

`conda update packageName`

###### Remove a package from a give environment:

`conda remove --name environmentName packageName`

###### Remove a package from the active environment:

`conda remove packageName`

