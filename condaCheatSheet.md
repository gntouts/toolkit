# Conda Cheatsheet
## Basic Conda 
Start conda:
<br>`conda init`<br><br>
Update conda:
<br>`conda update conda`<br><br>

## Environments
Create new environment with given Python version:
<br>`conda create -n environmentName python=3.6`
<br><br>
Activate given environment:
<br>
`conda activate environmentName`
<br><br>
Deactivate given environment:
<br>
`conda deactivate`
<br><br>
List all Conda environments:
<br>
`conda env list`
<br><br>
Remove an environment:<br>
(The environment must be inactive!)
<br>
`conda env remove --name environmentName`
<br><br>
## Packages
