# Stock Market Prediction Using Machine Learning
As part of the ML SIG Summer Project.
## Get Data
The Data is obtained from Quandl (restricted to the WIKI table) which requires an API key. The file get_data.py contains the necessary functions.

Usage:
```bash
python get_data.py [symbols]
```
For a list of available symbols for download, see: WIKI-datasets-codes.csv

## Features Used
* High-Low
* PCT_change
* MDAV5

### Structure of the repository
The repository houses:
* 'datasets' folder that is populated with stock data the first time script is run. To repopulate data:
  ```bash
  python get_data.py [quandl_symbol]
  ```
* 'research-papers' folder - the papers referred during the development of the model.
* 'environment.yml', 'requirements.txt' - [See this](#Setting-up-the-Environment) 
* 'WIKI-datasets-codes.csv' - A list of symbols to download data from Quandl.

### Running for the first time?
*The files environment.yml, requirements.txt make it easy to replicate the environment required for running the model.*
#### Setting up the Environment
1. For anaconda:<br>
   1. To install anaconda, [refer this](https://conda.io/docs/user-guide/install/index.html)<br>
   2. The base directory contains 'environment.yml' file. To replicate the same environment:
      ```bash
      conda env create -f environment.yml
      ```
2. For python3 virtual environment:<br>
   1. To install virtualenv, refer [this](https://www.digitalocean.com/community/tutorials/common-python-tools-using-virtualenv-installing-with-pip-and-managing-packages#a-thorough-virtualenv-how-to)
      ```bash
      pip install virtualenv
      virtualenv --python=python3 ml-stock-prediction
      ```
   2. The base directory contains 'requirements.txt' file. To install the required packages:
      ```bash
      pip install -r requirements.txt
      ```

## To-do:
1. Add functions to plot
