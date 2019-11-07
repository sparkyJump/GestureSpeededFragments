# GestureSpeededFragments

[**gsf.py**](gsf.py)  
A Python script to run the experiment, using [Psychopy](https://www.psychopy.org/). This is the file to run in order to start the experiment.

[mainTrials.xlsx](mainTrials.xlsx)  
Spreadsheet of trial types.

[mainTrials_test.xlsx](mainTrials_test.xlsx)  
Abbreviated spreadsheet of trial types. For quick test runs.

[plots.py](plots.py)  
A script to make some quick plots of the results, using [plotnine](https://plotnine.readthedocs.io/en/stable/).

[requirements.txt](requirements.txt)  
List of Python package versions used when developing the experiment. As produced by `pip freeze`. Use `pip install -r requirements.txt` to install all dependencies, for example in a new Python virtual environment. In particular note that Psychopy currently requires an older version of pyglet (1.3) than the latest (1.4), as per [this issue](https://github.com/psychopy/psychopy/issues/2518). You can force install the older version with `pip install 'pyglet<1.4' --force-reinstall`.

[data](data)  
Data collected in the experiment is saved here. *.psydat* files store Psychopy TrialHandler objects. These are saved even if the subject does not complete the experiment. *.csv* files store results from completed runs of the experiment.

[extras](extras)  
Miscellaneous additional files.

[gestures](gestures)  
*.mp4* video files with the gestures. Shown on screen during the experiment.

[plots](plots)  
Some plots of the results. Generated by [plots.py](plots.py).

[text](text)  
Text files of onscreen instructions.

[getPsychoPyCollectedData.R](getPsychoPyCollectedData.R)  
R script to collect the individual results and save one dataframe named collectedData.csv.
