# PSY2150-Skills-Workshop-2
## Overview
* This is an executive function experiment involving task switching. On each 
trial, participants will be presented a digit between 0-9 and a cue. If the cue
is O/E, participants will respond with odd or even based on the digit. If the 
cue is H/L, participants will respond high or low based on the digit. 
* There are four conditions in blocks of trials: all O/E trials, 
all H/L trials, half O/E trials then half H/L trials, and half H/L trials then 
half O/E trials.
* The presentation order of the blocks and trials within blocks are randomized.
* The whole experiemnt should take no longer than 5-7 minutes. 
* Once you finish the experiment, two CSV files will be downloaded at the same
time. One is the raw data file without filtering, one is a processed data file
that has irrelevant information filtered out.

CLICK HERE TO RUN THE EXPERIMENT FOR YOURSELF
https://jasonkchow.github.io/PSY2150-Skills-Workshop-2/experiment.html

The experiment starts with some brief instructions for each type of trial with
some practice trials. After the practice trials, the experiment will start.

## Trial structure
* Present a fixation cross
* Present the cue and the digit
* Wait for a response or for the trial to time out.
* Loop back up to to the top until the block is over.

## Materials and proecdure
The stimuli are digits from 0-9. On each trial, a digit is pseudorandomly 
selected. In each block, there are 12 trials with exactly half of the trials
having the correct response being odd or high and the other half having the
correct response being even or low. The cue is either O/E or H/L. There are a 
total of 48 test trials.There are two practice trials for each type of trial, 
one for each correct response, with feedback. The test trials do not have 
feedback. The block order and trials within blocks are randomized across 
participants. 

Default experiment parameters:
* Fixation time: 1000ms
* Trial time limit: 3000ms
* Response keys: [f, j]

Default parameters are defined near the top of the experiment file and can be
changed there in local copies of the experiment.

The experiment is created using jsPsych (https://www.jspsych.org/).

## Data dictionary
The filtered data CSV has the following columns:
* rt: response time in milliseconds, null if trial timed out
* response: the key pressed by the participant, null if trial timed out
* trial_tag: type of trial, either odd_even or high_low
* corr_res: the correct response for the trial
* digit: the digit presented
* block_type: the type of block, either OE, HL, OEHL, or HLOE
* time_elapsed: time elapsed since the start of the experiment in milliseconds
* sbj_id: the subject ID, randomly generated at the start of the experiment
* start_time: the time the experiment started
* seed: the random seed used to generate the experiment
* corr: whether the response was correct or not