[![pytest status](https://github.com/denisecailab/minian/workflows/pytest/badge.svg?branch=master)](https://github.com/DeniseCaiLab/minian/actions?query=workflow%3Apytest)
[![codecov](https://codecov.io/gh/DeniseCaiLab/minian/branch/master/graph/badge.svg)](https://codecov.io/gh/DeniseCaiLab/minian)
[![conda version](https://img.shields.io/conda/vn/conda-forge/minian.svg)](https://anaconda.org/conda-forge/minian)
[![documentation status](https://readthedocs.org/projects/minian/badge/?version=latest)](https://minian.readthedocs.io/en/latest/?badge=latest)

[![license](https://img.shields.io/github/license/denisecailab/minian)](https://www.gnu.org/licenses/gpl-3.0)
[![code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![commit style](https://img.shields.io/badge/commit_style-conventional-orange)](https://conventionalcommits.org)


# MiniAn

MiniAn is an analysis pipeline and visualization tool inspired by both [CaImAn](https://github.com/flatironinstitute/CaImAn) and [MIN1PIPE](https://github.com/JinghaoLu/MIN1PIPE) package specifically for [Miniscope](http://miniscope.org/index.php/Main_Page) data.

# Windows Setup Instructions (Recommended Method)

1. Clone the Github Repo locally: `git clone https://github.com/skisurfer13/Minian-Gu-Lab.git`
1. Change directory to Minian: `cd minian/`
1. Create a Conda local env: `conda env create -n minian -f environment.yml`
1. Activate conda env: `conda activate minian`
1. Fix Panel installation:
    * On Windows: Copy panel files from `.conda/envs/minian/site-packages/` to `.conda/envs/minian/Lib/site-packages/`
    * On Linux: Install panel with pip in minian conda environment: `pip install panel=0.8.0`
1. Install pywiz libraries with conda: `conda install -n minian -c pyviz pyviz_comms=2.2.1`
1. Install shot-scraper CLI tool in minian conda environment: `pip install shot-scraper`. Also run `shot-scraper install` 
1. Fire up jupyter: `jupyter notebook` and open the notebook "Minian_pipeline.ipynb"

# Mamba Installation Procedure

1. Run conda as admin
1. `conda create -y -n minian`
1. `conda activate minian`
1. `conda install -y -c conda-forge mamba`
1. `conda deactivate`
1. `conda activate minian`
1. `mamba install -y -c conda-forge minian`
1. `conda install python=3.8`
1. `mamba install -y -c conda-forge minian`
1. `conda activate minian`
1. `minian-install --notebooks`
1. `minian-install --demo`

# Documentation

MiniAn documentation is hosted on ReadtheDocs at:

https://minian.readthedocs.io/
This contains the documentation for the Original Minian Pipeline maintained by Cai Lab

This upgraded version of Minian is maintained by Pranav Sawant at The University of Texas at Dallas 

# Contributing to MiniAn

We would love feedback and contribution from the community!
See [the contribution page](https://minian.readthedocs.io/en/latest/start_guide/contribute.html) for more detail!

# License

This project is licensed under GNU GPLv3.
