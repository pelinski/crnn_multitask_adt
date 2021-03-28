# Evaluating a multi-task and a single-task CRNN model for Automatic Drum Transcription
This [notebook](automatic_drum_transcription.ipynb) is part of my final project for the Music Information Retrieval course of the Master in Sound and Music Computing from Universitat Pompeu Fabra in Barcelona. The report accompanying the notebook  can be found [here](report.pdf).

## Summary
Multi-task learning can improve the generalization and robustness of data-driven models, assuming a statistical relationships between the different tasks. Recent approaches to automatic drum transcription (ADT) have exploited the locally periodic nature of Western drum performances by training ADT systems jointly with the task of beat and downbeat detection. While most ADT vocabularies contain only the three most common drum instruments (kick-drum, snare-drum and hi-hat), training such models for larger vocabulary transcriptions encounters the difficulty that the available datasets do not offer a significant frequency of appearance of these less usual drum instruments. A recent approach by [Cartwright and and Bello](http://dafx2018.web.ua.pt/papers/DAFx2018_paper_60.pdf) trains a CRNN model with a synthetic dataset along with other existing datasets in order to balance the instrument occurrences. In this project, I compare the performance of the multi-task version of this CRNN model and its single-task version on the Groove MIDI Dataset.

## Setup environment
The jupyter notebook uses a conda environment that can be easily set up by running the following commands in the terminal:
```
CONDA_RESTORE_FREE_CHANNEL=1 conda env create -f environment.yml
```
and then:
````
conda activate rhythm
````
