# Python Virtual Environment Guide
A virtual environment is used to contain a specific Python interpreter and software libraries and binaries which are needed to support a project (library or application). These are by default isolated from software in other virtual environments and Python interpreters and libraries installed in the operating system.
## For Windows
### Install virtualenv
```powershell
pip install virtualenv
```
### Check Installation
To verify the installation of `virtualenv`:
```powershell
virtualenv
```
If virtualenv is not accessible, you may need to set the PATH environment variable. Use the following command to find the path:
```powershell
pip show virtualenv
```
Add the displayed path to your environment variables and restart the command line.
### Check Virtualenv Version
```powershell
virtualenv --version
```
### Create a Virtual Environment
Navigate to your working directory and create a virtual environment:
```powershell
cd <working_dir>
virtualenv <project_name>
```
Alternatively, you can use the conventional name `venv`:
```powershell
virtualenv venv
```
### Activate the Virtual Environment
Navigate into your virtual environment directory
```powershell
cd <project_name>
```
If you named it `venv`, use:
```powershell
cd venv
```
Activate the virtual environment:
```powershell
Scripts\activat
```
### Install Required Packages
Packages installed will be available only inside the current virtual environment:
```powershell
pip install <package-name>
```
To list the installed packages:
```powershell
pip list
```
### Deactivate the Virtual Environment
```powershell
Scripts\deactivate.bat
```
### Delete the Virtual Environment
To delete the virtual environment, remove the project folder:
```powershell
rmdir /s /q <project_name>
```
or if you used `venv`:
```powershell
rmdir /s /q venv
```
### Acknowledgments
This guide is intended for note-taking purposes, based on information from [Python documentation](https://docs.python.org) and other online resources.
