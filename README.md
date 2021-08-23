# Dartmouth ECoG Lab Automated Spike Detector

#### This repository contains a generic intracranial EEG (iEEG) preprocessing pipeline and an automated spike detector for the detection of intracranial IEDs. 
###### Our automated method consists of a template-matching algorithm and convolutional neural network (CNN) for the detection of intracranial IEDs (“AiED”). The final network had an F1-score of 0.95 (95% CI: 0.91-0.98) and an average Area Under the Receiver Operating Characteristic of 0.98 (95% CI: 0.96-1.00). 
###### More information can be found in the following publications: [Horak et al., 2015](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/9600/96000N/Implementation-and-evaluation-of-an-interictal-spike-detector/10.1117/12.2189248.full?SSO=1) and ADD NEW CITATION HERE.


## Brief description of notebooks:
#### "Preprocessing.ipynb"
###### This notebook was created to preprocess intracranial EEG data. Input is a .EDF iEEG file. Output is a .csv file containing the preprocessed iEEG.
#### "aied.ipynb" 
###### This notebook contains our automated spike detector. Before using this detector, please download the "model_aied.pt" file, containing our pretrained network, and indicate where this file is stored in the detector notebook.


## Sample data
#### "sample_eegdata.csv" 
###### This file contains preprocessed iEEG where rows correspond to unique channels and columns correspond to time points (fs = 200). 
#### "sample_finalspikes.csv"
###### This file contains the IEDs detected from the sample EEG file with our automated detector. 

