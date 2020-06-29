## Be a geoscience detective ##

<font color=green>In this repo I resume work done at the [2018 Geophysics Sprint](https://mycarta.wordpress.com/2019/02/07/geophysics-python-sprint-2018-day-2-and-beyond-part-ii) (orgainzed by Agile Scientific ahead of the Annual SEG conference), which resulted in the [error flag demo notebook](https://github.com/mycarta/in-bruges/blob/master/notebooks/Error_flag_demo.ipynb) in the repo [in-bruges](https://github.com/mycarta/in-bruges).  

<font color=green>I was inspired to go back to it after watching a Stanford University webinar titled [How to be a statistical detective](https://learn.stanford.edu/WBN-MED-STATS-On-Demand-2020-02-05_LP-OD-Registration-2020-02-11.html). 
    
#### I presented this work as a [lightning talk](https://www.youtube.com/watch?v=NtBDf7d7mwM) I gave at the [Transform 2020 virtual conference](https://transform2020.sched.com/) organized by [Software Underground](https://softwareunderground.org/).

With the tools I showcase, one can asses the quality of a prediction, from an Inversion or Machine Learning model, against ground truth (for example impedance) , by:

- Calculating the difference between prediction and ground truth at each sample
- Flagging statistically significant differences based on a user-defined distance (in deviation units) from either the mean difference or the median difference

<img src="https://github.com/mycarta/Be-a-geoscience-detective/blob/master/for%20readme/flaged.png">

- Further characterizing the error as percentage within a specific zone, and with a cofindence interval via Boostrapping

<img src="https://github.com/mycarta/Be-a-geoscience-detective/blob/master/for%20readme/Lower_zone.png">

<img src="https://github.com/mycarta/Be-a-geoscience-detective/blob/master/for%20readme/Upper_zone.png">
                                                                                                              

### Conda setup ####
To create the conda environment for this tutorial run:

```
conda env create -f environment.yml
```

### License ###
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/"> CC BY Creative Commons License</a>.
    
The figure used is copyright of the Canadian Society of Exploration Geophysicists.

#### Be-a-geoscience-detective ####
A notebook demonstrating how to quantitatively QC the reuslts of seismic inversion or other geophysical processes from a paper. 

##### To run the notebook interactively with Binder click on the button below: #####
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mycarta/Be-a-geoscience-detective/master)



