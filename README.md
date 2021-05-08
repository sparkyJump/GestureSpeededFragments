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
List of Python package versions used when developing the experiment. As produced by `pip freeze`. Use `pip install -r requirements.txt` to install all dependencies, for example in a new Python virtual environment.

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
R script to collect the individual results and save in one dataframe named collectedData.csv.

---
# How To Use

To run this application, you'll need [Python3](https://www.python.org/downloads/) and [PsychoPy3](https://www.psychopy.org/) installed on your computer.

## Option 1
You are using a Mac and have downloaded this application by selecting the green download code button.

In finder locate where the application landed:
```bash
GestureSpeededFragments-master
```
From the command line of the terminal type:
```bash
cd 
```
Note: There is a space after cd and it is important.
Then drag the GestureSpeededFragments-master folder **containing** gsf.py into the terminal and type: 
```bash
python3 gsf.py
```
Note: Copy and paste will not work.

To begin PsychoPy will expect a participant ID code and for you to pick one of the two conditions (S or G). 

# About the Author

I studied applied linguistics which introduced me to the inspiring world of open source software, evidence based research, and the beauty of collaboration for solving real world problems. My interests broadened from language teaching to the development of tools and procedures for investigating when and how gestures support learning. Through this I discovered an empty niche in the gesture community toolbox: a tool for measuring gesture based language learning which is robust enough to be used in applied research settings, but also precise enough for behavioral analysis, **and** that is also flexible in its functionality. You can read more about me and my projects [here](https://orcid.org/0000-0002-3696-7999).
