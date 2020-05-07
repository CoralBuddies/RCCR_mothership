# Mothership Hackathon - Coral Challenge
For Raising Coral Costa Rica, by the Coral Buddies. Info on https://mothershipmissions.com/coralreefsos

# Requirements
* ACOLITE (http://odnature.naturalsciences.be/remsem/software-and-data/acolite)
* python 3
* sentinelsat python package
* bokeh package for interactive plots
* sklearn and keras for the neural network

# "Alpha Version"
The repository that you are currently looking at, is the product of the Mothership Hackathon Coral Challenge.

The code is collected in a number of notebooks:
1. download_and_acolite.ipynb. This notebook queries (and possibly downloads) the data for a hardcoded region of interest, and then processes it using the ACOLITE algorithm, using settings as defined in the settings files found in this repo. This notebook is for the Golfo Dulce, and there is another notebook in this repo for Bahia Culbera (same code, using different coordinates).
2. resample_timeseries_and_average. This code takes the products of the previous notebook, and creates average maps and also timeseries for any given coordinate. 
3. resize_pngs.ipynb. For the Neural Network it was useful to export the png images created with ACOLITE in a smaller and consistent format. This notebook does that.
4. Neural_Network_prototype.ipynb. This trains the model that can detect if an observation is good or bad.
5. Time_Series_Kd490_inprogress.ipynb. Create the Bokeh interactive plot of the timeseries data.
6. Correlation_Plot_inprogress.ipynb. Create the Bokeh interactive plot for correlating the turbidity and the temperature data.

# Collaborating

Mostly, the directory structure should be self explanatory. 

We use git (via github) for our version control. 

Things that NEVER go into git:
* data
* credentials
Things that DON'T usually go into git:
* notebooks
* models

## adding your code to the git repo
* the default branch is develop, you are not allowed to commit directly to master or develop
* if you are working on the code, create a new branch, naming convention <your name>/<feature description>
* if happy, first pull latest version of develop using `git pull origin develop` and resolve any merge conflicts
* create pull request from your branch to develop


# Contributors
Gagan Reddy
Damiano Pellegrino
Larissa Koupriouchina
Jeroen Franse
