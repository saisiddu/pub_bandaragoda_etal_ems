# Software Instructions: Online and Personal Computer

## Online Modeling Instructions 

To open interactive Jupyter Notebooks with the CUAHSI JupyterHub server, go to the upper right corner of the resource page and click on 'Open With'. Select CUAHSI JupyterHub.  You will be connected to a virtual machine with the software environment required to execute the models.

Notebook 1: Educate by exploring rainfall driven hydrographs with Landlab: Explore_routing_tutorial.ipynb

Notebook 2: Replicate an experiment on a watershed subset within regional Landlab landslide model to explore fire impacts. The resource was originally derived from a reproducible demonstration of the landslide modeling results from: Strauch, R., Istanbulluoglu, E., Nudurupati, S. S., Bandaragoda, C., Gasparini, N. M., and Tucker, G. E.: (2018) A hydro-climatological approach to predicting regional landslide probability using Landlab, Earth Surf. Dynam. Discuss., https://doi.org/10.5194/esurf-6-49-2018:  Replicate_landslide_model_for_fire.ipynb

Notebook 3: Reuse ecohydrology model for exploring climate scenarios. The gridded meteorology forcings are pre-processed in the Notebook in NewMexico_observatory_gridmet.ipynb: Reuse_ecohydrology_observatory.ipynb

## Personal Computer Installation Instructions 

### Packages

The notebooks included in this resource require the following Python packages:

```
landlab 1.6.0
geopandas 0.5.0
dask 1.2.0
ogh 0.2.1
matlplotlib 3.0.3
pandas 0.24.2
ffmpeg 4.1.3
hs_restclient 1.3.3
```

To ensure that you have the correct packages and versions, run the following command(s) inside a Python terminal:

```
$ conda list
```

or 

```
$ pip list
```

### Creating a Working Environment

We recommend using Anaconda to create a fresh Python environment with all dependencies installed. After installing Anaconda, simply run the commands below with your desired environment name in place of `MY_ENVIRONMENT_NAME`:

```
conda create -n MY_ENVIRONMENT_NAME --file requirements.txt
```

activate the environment and start a jupyter server

```
source activate MY_ENVIRONMENT_NAME
jupyter notebook
```
### Debugging a Working Environment
Are you getting errors?  Here are some suggested steps. If you still have issues, email help@cuahsi.org or reach out to us (comment on this resource or see emails in HydroShare profiles) and we will invite you to the HydroShare Slack #landlab channel. 

Bug: PackagesNotFound

```
PackagesNotFoundError: The following packages are not available from current channels.
```

Reduce the number of packages that were not available by running the following command

```
conda config --append channels conda-forge
```

Bug: Conda vs.Pip Install

If you get errors for a few packages, remove them from the requirements.txt file until you successfully created the conda environment.

```
conda create -n MY_ENVIRONMENT_NAME --file requirements.txt
```

Any packages that didn't get installed during creation of conda environment can be pip installed separately in the newly created conda environment.
for example: 

```
pip install hs-restclient==1.3.3
```

### Reproducible Quote of the Day:

"The product of mental labor - science - always stands far below its value, because the labor-time necessary to reproduce it has no relation at all to the labor-time required for its original production."  Karl Marx


