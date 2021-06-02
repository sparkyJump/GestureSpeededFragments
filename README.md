# GestureSpeededFragments

<p align="center">
  <a href="#key-components">Key Components</a> •
  <a href="#how-to-use">How To Use</a> •
  <a href="#emailware">Emailware</a>
</p>

# Key Components

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

Note: the following instructions work for Mac OS and should work on Windows and Linux systems as well.

## New to GitHub and on a Mac?
Download this application by selecting the green download `code` button.

Inside Finder locate where the application landed by typing:
```bash
gsf.py
```
Open the Terminal from the command line and type:
```bash
cd 
```
Note: There is a space after cd and it is important.
Drag the GestureSpeededFragments-master folder you just found **containing** gsf.py into the terminal and press enter.
Then type: 
```bash
python3 gsf.py
```
and press enter.
Note: Copy and paste will not work.

## Familiar with GitHub?

Clone this repository and set as working directory. 
You need to install the python3 development libraries first.
(This set of commands was tested with openSuse 15.1.)

For apt (Ubuntu, Debian...)
```bash
sudo apt-get install python3-dev  # for python3.x installs
```
For yum (CentOS, RHEL...)
```bash
sudo yum install python3-devel   # for python3.x installs
```
For dnf (Fedora...)
```bash
sudo dnf install python3-devel  # for python3.x installs
```
For zypper (openSUSE...)
```bash
sudo zypper install python3-devel  # for python3.x installs
```
For apk (Alpine...)
```bash
sudo apk add python3-dev  # for python3.x installs
```
For apt-cyg (Cygwin...)
```bash
apt-cyg install python3-devel  # for python3.x installs
```
Start up a virtual environment and install the python3 dependencies with pip. (Tested with openSuse 15.1.)
```bash
$ python3 -m venv env
$ source env/bin/activate
(env)$ pip install six
(env)$ pip install appdirs
(env)$ pip install packaging
(env)$ pip install ordered_set
(env)$ pip install -r requirements.txt
(env)$ python3 gsf.py
```

# Experiment Protocol

To begin PsychoPy will expect you to enter a participant ID code and for you to pick one of the two gesture conditions. If you have not modified the task then you have two conditions (S or G) as explained in the [project description](https://github.com/natashajanzen/GestureSpeededFragments/projects). 
The time needed for all 32 items in both conditions is usually 10-12 minutes. This is for children learning English as a second language who are age 10-12. Younger children would need more time. Adults may require slightly different instruction, such as additionally asking them to "carefully follow the hand movements". 

# Emailware

The gesture speeded fragment completion task is an [emailware](https://en.wiktionary.org/wiki/emailware). This means  that if you liked using this app or it has helped you in any way, I'd like you to send me an email at <hedgewood@gmail.com> with anything you'd want to say about this software. I'd really appreciate it!

# About the Author

I studied applied linguistics which introduced me to the inspiring world of open source software, evidence based research, and the beauty of collaboration for solving real world linguistic problems. My interests broadened from language teaching to the development of tools and procedures for investigating when and how gestures support learning. Through this I discovered an empty niche in the gesture community toolbox: a tool for measuring changes in gesture perception which is robust enough to be used in applied research settings, but also precise enough for behavioral analysis, **and** that is also flexible in its functionality. You can read more about me and my projects [here](https://orcid.org/0000-0002-3696-7999).
