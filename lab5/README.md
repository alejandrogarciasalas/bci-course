# Lab 5: SSVEP

### Introduction
In this lab, we will record EEG while trying to remember words, as well as later recognizing these same words among others. Hopefully, we'll be able to see the event related potentials corresponding to remembered vs not-remembered words, and possibly recognized vs not recognized words.

### Setup

First, install the libraries:
``` bash
npm install
pip install -r requirements.txt
```

(If you don't have `npm`, you can install by running `brew install node`. You can get `brew` from https://brew.sh/)

### Stimulus Presentation + Recording


- Attach electrodes to participant's head, preferably in visual cortex on the back of the head. 
- Have participant sit in chair in front of monitor
- Connect to the ganglion and stream data: `node ganglion-lsl.js`
- Run lsl-viewer to check connections and stream: `python lsl-viewer.py`
- Run SSVEP stimulus: `python stimulus_one.py`
- Record data: `python lsl-record.py -f data/data_20hz.csv`
- Change the frequency of stimulus (edit `freq = 20` in stimulus_one.py to some other frequency)
- Record a few more

- Look at the data by opening the notebook!


