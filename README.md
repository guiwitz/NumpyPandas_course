[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/guiwitz/NumpyPandas_course/54488164b462644baf601875be69cc911eda9615?urlpath=lab)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guiwitz/NumpyPandas_course/blob/colab)


# Introduction to Numpy and Pandas

This repository contains Jupyter notebooks introducing beginners to the Python packages Numpy and Pandas. The material has been designed for people already familiar with Python but not with its "scientific stack".

This material has been created by Guillaume Witz (Science IT Support, Microscopy Imaging Center, Bern University) in the frame of the [courses offered by ScITS](https://www.scits.unibe.ch/).

## Content
The course has the following content:

### Numpy
- [Numpy arrays:](01-DA_Numpy_arrays_creation.ipynb): what they are and how to create, import and save them
- [Maths with Numpy arrays](02-DA_Numpy_array_maths.ipynb): applying functions to arrays, doing basic statistics with arrays
- [Numpy and Matplotlib](03-DA_Numpy_matplotlib.ipynb): Basics of plotting Numpy arrays with Matplotlib
- [Recovering parts of arrays](04-DA_Numpy_indexing.ipynb): Using array coordinates to extract information (indexing, slicing)
- [Combining arrays](05-DA_Numpy_combining_arrays.ipynb): Assembling arrays by concatenation, stacking etc. Combining arrays of different sizes (broadcasting)
  
### Pandas
- [Introduction to Pandas](06-DA_Pandas_introduction.ipynb): What does Pandas offer?
- [Pandas data structures](07-DA_Pandas_structures.ipynb): Series and dataframes
- [Importing data to Pandas](08-DA_Pandas_import_plotting.ipynb): Importing data tables into Pandas (from Excel, CSV) and plotting them
- [Pandas operations](09-DA_Pandas_operations.ipynb): Applying functions to the contents of Pandas dataframes (classical statistics, ```apply``` function etc.)
- [Combining Pandas dataframes](10-DA_Pandas_combine.ipynb): Using concatenation or join operations to combine dataframes
- [Analyzing Pandas dataframes](11-DA_Pandas_splitting.ipynb): Split dataframes into groups (```groupy```) for category-based analysis
- [A real-world example](12-DA_Pandas_realworld.ipynb): Complete pipeline including data import, cleaning, analysis and plotting and showing the nitty-gritty issues one often faces with real data

## Running the course

### Live sessions

During live sessions of the course, you are given access to a private Jupyter session and don't need to install anything no your computer.

### Without installation
Outside live-sessions, this entire course can still be run interactively without any local installation thanks to the [mybinder](mybinder.org) service. For that just click on the mybinder tag at the top of this Readme. This will open a Jupyter session for you with all packages, notebooks and data available to run.

Alternatively you can also run the course on Google Colab. For that just click on the Colab badge at the top of this file.

### Local installation
For a local installation, we recommend using conda to create a specific environment to run the code. If you don't yet have conda, you can e.g. install miniconda, see [here](https://docs.conda.io/en/latest/miniconda.html) for instructions. Then:

1. Clone the repository to your computer using [this link](https://github.com/guiwitz/NumpyPandas_course/archive/master.zip) and unzip it
2. Open a terminal and move to the ```NumpyPandas_course-master/binder``` folder
3. Here you find an ```environment.yml``` file that you can use to create a conda environment. Choose an environment name e.g. ```numpypandas``` and type:
   ```
   conda env create -n numpypandas -f environment.yml
   ```
4. When you want to run the material, activate the environment and start jupyter:
   ```
   conda activate numpypandas
   jupyter lab
   ```
   Note that the top folder of your directory in Jupyter is the folder from where you started Jupyter. So if you are e.g. in the ```binder``` folder, move one level up to have access to the notebooks

## Note on the data used

In the Pandas part, we use some data provided publicly by the Swiss National Science foundation at this link: http://p3.snf.ch/Pages/DataAndDocumentation.aspx#DataDownload. The examples of analysis on these data **are in no way confirmed or validated by the SNSF and are entirely the work of Guillaume Witz, Science IT Support, Bern University**.

