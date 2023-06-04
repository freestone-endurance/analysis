# Freestone Endurance Analyses

## High Lonesome 100 Cutoff Analysis

**Goal**: Evaluate the "fairness" of High Lonesome 100 cutoffs.
**Timeline**: Done in 2023 prior to 2023 running.

See [CutoffAnalysis2023](analyses/CutoffAnalysis2023.ipynb)

## Development ##

### Simple Setup ###

First install python dependencies:

```
pip install jupyterlab -r ./requirements.txt
```

### Conda Setup ###

Create a jupyterlab conda environment with python 3.8:

```
conda create -n jupyterlab python=3.8
conda activate jupyterlab
pip install jupyterlab
```

Create an analysis conda environment and tell the ipython kernel about it:

```
conda create -n analysis python=3.11
conda activate analysis
pip install -r requirements.txt
conda install nb_conda_kernels
ipython kernel install --user --name=cutoff-analysis
```

### Running the Notebook ###

Now with the environment that you installed `jupyterlab` in, run `jupyter-lab`. Then navigate to the local URL and open up the notebook!
