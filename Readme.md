# Introduction

Unfortunately, pyStan 3 is not compatible with Windows/Mac by default. However, this repository provides a containerized version that can be used on any environment. Users can add Python scripts in the `./stan/` directory.

This repository is intended to use with cookie-cutter and VSCode, fully exploiting the devcontainers that allows you to run pyStan 3 in a container, but work on it through the VSCode seamelessly like if it was installed on your machine.

## Installation

## General setup

- Install wsl (linux system for windows) https://learn.microsoft.com/en-us/windows/wsl/install
- Reboot computer
- Install docker https://docs.docker.com/desktop/install/windows-install/
- Reboot computer
- install python3 if not yet installed https://www.python.org/downloads/
- Using command line, install cookie-cutter (`pip install cookiecutter`)
- Install VSCode: https://code.visualstudio.com/download
- Install in VSCode the extension `Dev Containers` by Microsoft


## Creation of a project using this template

- install this repo using cookiecutter: `cookiecutter gh:dbonattoj/cookiecutter-pystan.git`


If VSCode asks for a python interpreter, select `/usr/local/bin/python3` (it should be the 3.10 version)


# Usage

In VSCode, use `Connect to` > `Open folder in container` and select the folder where you installed the project.

This will automatically create the docker image, and you'll be able to directly edit scripts (folder: `stan`) and jupyter notebooks (folder:``notebooks`) and execute them in VSCode.