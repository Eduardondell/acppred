# acppred

By Eduardo Dellagostin

a tool to predict anticancer peptides. This tool was structured during the Software Engeneering applied to Bioinformatics and Machine Learning course of the PPG Biothecnology from UFPel.

## Setup

```
$ make setup
```
## Project structure

environment.yml -> channels and dependencies utilized 

requirements.txt -> all the dependencies requirements for running

Makefile -> short command for running the environment

models.py -> file with the code to a predictive model for anticancer peptides, it utilizes a database with positive and negative peptides obtained from antiCP platform. This file contains the core of ACPPred tool.

predict.py -> file containing the predictive tool for anticancer peptides. This code loads the trained model and use its parameters to predict the anticancer potential for an inputed sequence. Returning the result with a probability of the anticancer activitiy of the peptide.

train.py -> Trains the model for predicting anticancer peptides. It uses the Random Forest Classifier from scikit learn to estimate the positive and negative peptides. 


