# applied_machine_learning_project
This my third project in the capstone course of Udacity's Master's Degree in AI (https://www.udacity.com/masters-artificial-intelligence). 

## Overview
In this project, we complete a full machine learning workflow for a dataset on whine quality (https://archive.ics.uci.edu/dataset/186/wine+quality). 
This dataset contains two csv files on chemical properties and quality scores of red and white whines, respectively. We will focus on the white wine data in this project (file <i>winequality-white.csv</i>).

We start by loading, cleaning and rescaling the data. We then try to classify the quality using the chemical properties by fitting a decision tree model. 
We apply regularization techniques to avoid overfitting, evaluate the model performance, and conclude by a short summary of our findings.

## How to run the project
The main component of the project is the Jupyter notebook 'modeling.ipynb'.
When checking out this repository, the dataset file 'train.csv' is already included.
In addition, the repository contains a 'requirements.txt' file with all required dependencies, which was generated via the command
	
	pip freeze > requirements.txt
	
It can be used e.g. in a virtual Anaconda environement by opening an Anaconda prompt window in the project directory and running the following commands:

	conda create -n env_msai_cap_3 python
	conda activate env_msai_cap_3
	pip install -r requirements.txt
	python -m ipykernel install --user --name=env_msai_cap_3
	jupyter notebook
	
The last command opens a Jupyter GUI, where one needs to click on the notebook 'modeling.ipynb' and then click on Run... -> Run All Cells
