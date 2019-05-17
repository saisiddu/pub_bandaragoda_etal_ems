# pub_bandaragoda_etal_ems
The problem: Researchers need a modeling workflow that is flexible for developing their own code, with easy access to distributed datasets, shared on a common platform for coupling multiple models, usable by science colleagues, and with easy publication of data, code, and scientific studies.

The emerging solution: Collaborate with the CUAHSI HydroShare community to use and contribute to water data software and hardware tools, so that you can focus on your science, be efficient with your time and resources, and build on existing research in multiple domains of water science.

# Citation instructions
### Journal publication
Bandaragoda, C. J., A. Castronova, E. Istanbulluoglu, R. Strauch, S. S. Nudurupati, J. Phuong, J. M. Adams, et al. “Enabling Collaborative Numerical Modeling in Earth Sciences Using Knowledge Infrastructure.” Environmental Modelling & Software, April 24, 2019. https://doi.org/10.1016/j.envsoft.2019.03.020.

### Data and code publication
Bandaragoda, C., A. M. Castronova, J. Phuong, E. Istanbulluoglu, S. S. Nudurupati, R. Strauch, N. Lyons (2019). Enabling Collaborative Numerical Modeling in Earth Sciences using Knowledge Infrastructure: Landlab Notebooks, HydroShare, http://www.hydroshare.org/resource/70b977e22af544f8a7e5a803935c329c

These Notebooks are designed to run on HydroShare (see below). To view the Notebook code (without interactive capabilities), use the Notebooks in this Github repository (Code folder).  To run the Notebooks on your personal computer, please see installation recommendations below.   To develop and update the Notebooks, please fork this repository and use Issues to keep in touch. Commits with quotes are much appreciated! 

Spread love everywhere you go. Mother Teresa

# Run the Notebooks on HydroShare
Interactive Landlab notebooks are available on HydrosShare at http://www.hydroshare.org/resource/70b977e22af544f8a7e5a803935c329c. These Jupyter Notebooks are designed to introduce users to Landlab modeling framework on the [CUAHSI](www.cuahsi.org) [JupyterHub server](https://jupyter.cuahsi.org).  

To run the Notebooks on HydroShare, Sign up or Sign in at www.hydroshare.org.   
When you [click on this resource](http://www.hydroshare.org/resource/70b977e22af544f8a7e5a803935c329c) you will see a blue 'Open With' in the top right corner.  Select the CUAHSI JupyterHub server from the dropdown list. You will be connected to a virtual machine with the software environment required to execute the models.  Once the data is transferred, you can click on each of the Notebooks. 

Notebook 1: Educate by exploring rainfall driven hydrographs with Landlab
Explore_routing_tutorial.ipynb

Notebook 2: Watershed subset within regional Landlab landslide model to explore fire impacts
Replicate_landslide_model_for_fire.ipynb
The resource was originally derived from a reproducible demonstration of the landslide modeling results from: Strauch, R., Istanbulluoglu, E., Nudurupati, S. S., Bandaragoda, C., Gasparini, N. M., and Tucker, G. E.: (2018) A hydro-climatological approach to predicting regional landslide probability using Landlab, Earth Surf. Dynam. Discuss., https://doi.org/10.5194/esurf-6-49-2018.

Notebook 3: Reuse ecohydrology model for exploring climate scenarios
Reuse_ecohydrology_observatory.ipynb
The gridded meteorology forcings are pre-processed in the Notebook in NewMexico_observatory_gridmet.ipynb.

# Installation Instructions to run the Notebooks on a personal computer


## Packages

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

## Creating a Working Environment

We recommend using Anaconda to create a fresh Python environment with all dependencies installed. After installing Anaconda, simply run the commands below with your desired environment name in place of `MY_ENVIRONMENT_NAME`:

```
conda create -n MY_ENVIRONMENT_NAME --file requirements.txt
```

activate the environment and start a jupyter server

```
source activate MY_ENVIRONMENT_NAME
jupyter notebook
```


