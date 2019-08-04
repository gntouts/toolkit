# Conda Cheatsheet
## Basic Conda 
###### Start conda:
<br>`conda init`<br><br>
###### Update conda:
<br>`conda update conda`<br><br>

## Environments
###### Create new environment with given Python version:
<br>`conda create -n environmentName python=3.6`
<br><br>
###### Activate given environment:
<br>
`conda activate environmentName`
<br><br>
Deactivate given environment:
<br>
`conda deactivate`
<br><br>
###### List all Conda environments:
<br>
`conda env list`
<br><br>
###### Remove an environment:<br>
(The environment must be inactive!)
<br>
`conda env remove --name environmentName`
<br><br>
## Packages
###### List all packages and versions in active environment:
<br>
`conda list`
<br><br>
###### Search a package to check if it is possible to install:
<br>
`conda search packageName`
<br><br>
###### Install a package in a given environment:
<br>
`conda install -n environmentName packageName`
<br><br>
###### Install a package in the active environment:
<br>
`conda install packageName`
<br><br>
###### Update a package in the active environment:
<br>
`conda update packageName`
<br><br>
###### Remove a package from a give environment:
<br>
`conda remove --name environmentName packageName`
<br><br>
###### Remove a package from the active environment:
<br>
`conda remove packageName`
<br><br>
