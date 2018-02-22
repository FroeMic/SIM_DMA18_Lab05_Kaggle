# DMA18 Lab 05 Kaggle Competition


https://www.kaggle.com/c/cal-dma-2018
Invite Link: https://www.kaggle.com/t/b176d1b772f64e2c9854aa7bfa8a0a2f

## How to contribute

[1] Use precise and meaningful commit message that tell the others what was changed.

[2] Respect the folder structure.

```
- /data/ .............. (the extracted data from the kaggle competition. in .gitignore)
- /models/ ............ (stored models)
- /src/ ............... (put iphython notebooks here)
```

## Getting Started

### [1] Download the data

The `/data/` folder is in the `.gitignore` meaning that nothing it is pushed to the remote repository.
After cloning the repository, download and extract the source data from https://www.kaggle.com/c/cal-dma-2018/data into the `/data/` folder. 

### [2] Bootstrap Environment
To start you will need **virtualenv**, to bootstrap our environment.
It's a more flexible way  of managing environments as opposed to anaconda.

#### Intitial Installation

Do this one time: Run the following commands

```
pip install virtualenv
virtualenv --python=/usr/local/bin/python3 .lab05
source .lab05/bin/activate
pip install -r requirements.txt
```

Then start jupyter (`jupyter notebook`) and check, whether everything works by running all cells in the `AssertInstallation.ipynb`.

#### Activate environment

Do this everytime.

```
source .lab05/bin/activate
```

#### Installing new packages

Do this everytime you use `pip install` within the environment to install a new package.
It saves all required packages into the `requirements.txt` file, which you should push to the remote repository then.

```
pip freeze > requirements.txt
```
