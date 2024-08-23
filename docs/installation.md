# Software installation

Conda is an open-source package and environment management system that runs on Windows, macOS, and Linux. The conda repository contains a large number of open-source certified packages enabling scientific work. It is recommended that you install the minimal installer for conda named miniconda that includes only conda, Python, the packages they depend on, and a small number of other useful packages, including pip, zlib and a few others.

## Download and install miniconda

Retrieve miniconda from the following website

> <https://docs.conda.io/en/latest/miniconda.html>

Install the version for 64 bit computers.

**OBS** for MacOS, there are different downloads for intel and M1 processors. Follow these steps to find out what is on your laptop:
1. Click the Apple icon in the top-left corner of your Mac.
2. This will bring up a drop-down menu. Pick the top option: About This Mac.
3. The resulting window should show you the information you need: look for ```intel``` or ```M1```

## Create conda environments and install packages

### All in one step

Get all packages needed for course in one step with use of a YML file

```
(base) % conda env create -f cb1020.yml
```

where the file [`cb1020.yml`](../cb1020.yml)* contains

```
name: cb1020
channels:
  - conda-forge
dependencies:
  - python
  - jupyterlab
  - jupyterlab-spellchecker
  - jupyterlab_code_formatter
  - black
  - isort
  - numpy
  - scipy
  - matplotlib
  - mesa
  - pandas
  - pyarrow
  - openpyxl
  - pytorch
  - torchvision
```

Some additional features are then made available in your notebooks such as a spell checker and a Python code formatter.

***OBS** simply download the file, do not open it!

### Step-by-step

Start a conda terminal, or Anaconda Powershell as it is referred to on a Windows system. Conda supports multiple *environments* and you start in the one named `base` as is typically indicated by the prompt. To create a new and additional environment named `cb1020`, enter the following command line statement

```
(base) % conda create -n cb1020
```

You can list your conda environments

```
(base) % conda env list
```

The activated environment will be marked with an asterisk (the `base` environment to begin with) and you can activate your new environment with the command

```
(base) % conda activate cb1020
```

as should be indicated by getting a modified prompt.

Install packages into this environment

```
(cb1020) % conda install numpy scipy matplotlib jupyterlab mesa -c conda-forge
```

```{admonition} Good practices
:class: note

- Never install any additional packages in the `base` environment. Keep it minimal and clean and thereby minimize the risk for package conflicts. 

- At times, update the conda package manager <br>
`(base) % conda update conda`

- At times, clean up among downloaded packages <br>
`(base) % conda clean --all` <br>
This command will not remove any functionality but for most parts remove tarball files. 

```

## Try it out

You should now be ready to start JupyterLab with the commands

```
(base) % conda activate cb1020
(cb1020) % jupyter-lab
```

which should open the web browser interface.