## Setup and Installation Instructions for the Workshop


To download and execute the notebooks, we recommend you clone the 
aas239-jwebbinar repository to your local computer. 
You will then want to install all associated packages necessary to run the notebooks. 
These packages can be installed using pip.
You will need python version **3.8.10**. We recommend the 
following command sequence:

```   
% git clone https://github.com/spacetelescope/jdat_notebooks.git
% cd jdat_notebooks/notebooks/<whatever-notebook>
% conda create -n jwebbinar python=3.8.10
% conda activate jwebbinar
% pip install -r pre-requirements.txt
% pip install -r requirements.txt
% pip install jupyter
% jupyter notebook
```

For the commands shown, `%` (and anything to the left of it) represents the
terminal prompt. You do not need to copy it; instead only copy the command to the
right of `%`.

## Install Miniconda (if needed)

*Miniconda is a free minimal installer for conda. It is a small, bootstrap
version of Anaconda that includes only conda, Python, the packages they depend
on, and a small number of other useful packages, including pip, zlib and a few
others. Note, though, that if you have either Miniconda or the full Anaconda
already installed, you can skip to the next step.*

In a terminal window, check if Miniconda is already installed.

    % conda info

If Miniconda is not already installed, follow these instructions for your
operating system: https://conda.io/projects/conda/en/latest/user-guide/install/index.html.
Please be sure to install a **64-bit version** of Miniconda to ensure all packages work correctly.


