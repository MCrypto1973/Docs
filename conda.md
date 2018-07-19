# Managing conda
### Find conda version
- conda --version
### Update conda
- conda update conda

# Managing Environment
### Create a new conda environment and install package in it
- conda create --name <environment_name> <package_name>
### List environment:
- conda info --envs
### Change environment:
- activate <environment_name>
### Return to base environment:
- deactivate
### Remove conda environment
- conda env remove --name <environment_name>

# Managing Package
### List package from Anaconda repository
- conda search <package_name>
### Install package
- conda install <package_name>
### List packages from environment
- conda list
