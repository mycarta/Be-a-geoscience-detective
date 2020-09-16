## Be a geoscience detective ##

In this repo I resume work done at the [2018 Geophysics Sprint](https://mycarta.wordpress.com/2019/02/07/geophysics-python-sprint-2018-day-2-and-beyond-part-ii) (organized by Agile Scientific ahead of the Annual SEG conference), which resulted in the [error flag demo notebook](https://github.com/mycarta/in-bruges/blob/master/notebooks/Error_flag_demo.ipynb) in the repo [in-bruges](https://github.com/mycarta/in-bruges).  

The inspiration came after watching [How to be a statistical detective](https://learn.stanford.edu/WBN-MED-STATS-On-Demand-2020-02-05_LP-OD-Registration-2020-02-11.html), a Stanford University webinar.
    
#### I presented this work as a [lightning talk](https://www.youtube.com/watch?v=NtBDf7d7mwM) I gave at the [Transform 2020 virtual conference](https://transform2020.sched.com/) organized by [Software Underground](https://softwareunderground.org/).

The notebook demonstrates how one can asses the quality of multiple predictions against one another (from Inversions and/or Machine Learning models) and against ground truth (for example from geophysical logs), by:

1. Calculating the difference between prediction and ground truth at each sample
2. Flagging statistically significant differences based on a user-defined distance (in deviation units) from either the mean difference or the median difference

<img src="https://github.com/mycarta/Be-a-geoscience-detective/blob/master/for%20readme/flaged.png">

3. Further characterizing the error as percentage within a specific zone, and with a cofindence interval via Boostrapping

<img src="https://github.com/mycarta/Be-a-geoscience-detective/blob/master/for%20readme/table.png">

<img src="https://github.com/mycarta/Be-a-geoscience-detective/blob/master/for%20readme/Lower_zone.png">

<img src="https://github.com/mycarta/Be-a-geoscience-detective/blob/master/for%20readme/Upper_zone.png">
                                                                                                              

### Conda setup ####
To create the conda environment for this tutorial run:

```
conda env create -f environment.yml
```

### License ###
The figure used is copyright of the Canadian Society of Exploration Geophysicists.

The rest is open source, and copyright of Matteo Niccoli, 2020:

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />Text is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/"> CC BY Creative Commons License</a>.

Code is Licensed under the [Apache License, Version 2.0]( http://www.apache.org/licenses/LICENSE-2.0).

#### Be-a-geoscience-detective ####
A notebook demonstrating how to quantitatively QC the reuslts of seismic inversion or other geophysical processes from a paper. 

##### To run the notebook interactively with Binder click on the button below: #####
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mycarta/Be-a-geoscience-detective/master)



