## Setup and Installation Instructions for the Workshop

To download and execute the notebooks, we recommend you clone the 
aas239-jwebbinar repository to your local computer. 
You will then also need to install all associated packages necessary to run the notebooks.
To facilitate this, we describe each of the steps below.

For the commands shown below, `%` (and anything to the left of it) represents the terminal prompt.
You do not need to copy it; instead only copy the command to the right of `%`.

## 0. (Optional, only for Windows) Install WSL

*If you are using Windows, you have two possible ways to install Python and Conda.  One option is to use the native windows installer for Miniconda (detailed below), but you can also use the Windows Subsystem for Linux (WSL) instead of using native Windows tools. WSL is now fully supported by Microsoft and tends to result in fewer install headaches, because it lets you use tools that were developed for Linux in Windows. You can try either approach as you prefer, but if you want to try WSL you'll need to follow this step first, and then from here on work like you are on Linux instead of Windows.*

To install WSL, you should follow the instructions Microsoft provides here: https://docs.microsoft.com/en-us/windows/wsl/install. While you may choose an alternative Linux distribution from the default Ubuntu, the instructions below have been tested on Ubuntu, so unless you have a specific reason, we suggest you stick with the default.  Once you reach the point in the instructions with a working Linux terminal prompt, you can proceed to step 1 of these instructions.

*Optional* While you can run a WSL terminal with the command prompt built into Windows, it's rather bare-bones and you may not have the best experience.  For WSL on Windows you'll probably want to [install Windows Terminal](https://docs.microsoft.com/en-us/windows/terminal/install) to have a terminal experience closer to what you'd see on Mac or Linux.


## Step 1: Install Miniconda (if needed)

*Note: if you already have familiarity with Python and a working installation of conda you prefer to use, you may be able to skip this step.*

*Miniconda is a free minimal installer for conda. It is a small, bootstrap
version of Anaconda that includes only conda, Python, the packages they depend
on, and a small number of other useful packages, including pip, zlib and a few
others. Note, though, that if you have either Miniconda or the full Anaconda
already installed, you can skip to the next step.*

In a terminal window, check if Miniconda is already installed.

```
% conda info
```

If Miniconda is not already installed, follow these instructions for your
operating system: https://conda.io/projects/conda/en/latest/user-guide/install/index.html.
Please be sure to install a **64-bit version** of Miniconda to ensure all packages work correctly.


## Step 2: Clone the aas239-jwebbinar repository

If you do not have git installed you will need to [install git]().  Once you have done this, you can do:

```   
% git clone https://github.com/spacetelescope/aas239-jwebbinar.git
% cd aas239-jwebbinar/00_Installation
```

## Step 3: Install the requirements

These packages are reqorded in the requirements files in this directory, and can be installed using pip.

You will need python version **3.8.10**. 
We recommend using the following command sequence to creates a conda environment and prepare it for installation  

```
% conda create -n aas239-jwebbinar python=3.8.10 pip wheel numpy
% conda activate aas239-jwebbinar
% pip install -r pre-requirements.txt
```

Afterwards, please install the main requirements file. If you are on a Windows machine (not installing within the Windows Subsystem for Linux), please run our specific windows requirements file
```
% pip install -r requirements_windows.txt
```

Otherwise, on macOS or a Linux distribution (or on Windows within a Windows Subsystem for Linux):
```
% pip install -r requirements.txt
```

## Step 4: Verify Installation

Run the `ValidateEnvironment.ipynb` notebook to test that your installation works.

```
% cd ..
% jupyter notebook ValidateEnvironment.ipynb
```

From the menu choose *Kernel* and then *Restart and Run All*.  If the last cell runs, you are good to go.