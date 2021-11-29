## Setup and Installation Instructions for the Workshop

To download and execute the notebooks, we recommend you clone the 
aas239-jwebbinar repository to your local computer. 
You will then also need to install all associated packages necessary to run the notebooks.
To facilitate this, we describe each of the steps below.

For the commands shown below, `%` (and anything to the left of it) represents the terminal prompt.
You do not need to copy it; instead only copy the command to the right of `%`.

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
% cd aas239-jwebbinar
```

## Step 3: Install the requirements

These packages are recorded in the requirements files in this directory, and can be installed using pip.

We recommend the following command sequence, which creates a conda environment and installs the requirements into it.  

**Note: these commands will install version 3.9 of Python. Other versions of Python may work, but have not been thoroughly tested, so they may or may not work for you.**

```
% conda create -n aas239-jwebbinar pip wheel numpy scipy bottleneck python=3.9
% conda activate aas239-jwebbinar
% pip install -r 00_Installation/pre-requirements.txt
% pip install -r 00_Installation/requirements.txt
```

If you follow the above instructions, any time you open a new terminal you *must* do:
```
% conda activate aas239-jwebbinar
```
for your installed packages to get used by Python.