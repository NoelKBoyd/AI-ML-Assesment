# Artificial Intelligence and Machine Learning

An end-to-end machine learning workflow for analysing and predicting road collisions in Sheffield.

## Prerequisites

Before you begin, make sure you have the following installed:

- [Python 3.12](https://www.python.org/downloads/release/python-3120/) — **other versions are not supported** (TensorFlow requires Python 3.12 or below)
- [VS Code](https://code.visualstudio.com/) with the **Python** and **Jupyter** extensions installed
- [Git](https://git-scm.com/)

## Setup Guide

### 1. Clone the repository

git clone <https://github.com/NoelKBoyd/AI-ML-Assesment>

### 2. Create a virtual environment using Python 3.12

py -3.12 -m venv venv

### 3. Activate the virtual environment

**Windows:**

venv\Scripts\activate

**Mac/Linux:**

source venv/bin/activate

You should see `(venv)` appear at the start of your terminal prompt.

### 4. Install dependencies

pip install -r requirements.txt

## File organisation

The repository is organised into: data, notebooks and results. Data stores the original traffic data then any subsequent datasets for example the preprocessed traffic data is a subset of that original after its been 'cleaned'. Notebooks contains each criterion from 1-6 each dedicated to a different part of the criterion. Lastely results contains all of the graphs used for analysis that is created from the jupyter notebooks.

## Usage

Each notebook (Criterion 1-6) can be ran using your virtual environment, to use your virtual click the jupyter notebook you wish to run and in the top right you can select your kernal, make sure to click the venv that you have just installed your dependencies to.

## Artificial Intelligence Transparency Decleration Statement

I used AI at Level 2 (AI for Shaping) of the Artificial Intelligence Transparency Scale (AITS). Specifically, I used Gemini to help brainstorm initial ideas and outline the structure of my GitHub repository. My own contribution involved developing all arguments, conducting research, writing the full code, and critically evaluating the structure suggested by the AI. I used AI as a thinking partner to shape my approach, but all substantive content and analysis are my own. I only used AI to improve the conciseness and professionalism of my text, not to conduct the actual analysis itself.

## AI Prompts / logs:

1.

Prompt "How can I carry across my pre-processed data in C1 to C2 so that the dataframe is still defined in C2"

Response: Jupyter Notebooks run in completely isolated memory environments called kernels. Save the data at the end of Criterion 1 and Load the data at the start of Criterion 2.

Code:

df.to_csv("../data/Preprocessed_Traffic_Data.csv", index=False) #save data

df = pd.read_csv("../data/Preprocessed_Traffic_Data.csv", low_memory=False) #load data

2.

Prompt "Can you suggest improvements to the analysis sections of my markdown to increase the readability, do not change my analysis verdicts but make improvements"

Response jist: improved a few cells of my markdown just to make it clearer and a bit more professional / concise as I do tend to ramble in my explanations as well as improving the use of specific terminology.

3.

Prompt "Can you suggest some clearer comments for my code so that my lecturer has an easier time stepping through each cell"

Response jist: improved my comments as before it was mainly short explanations with no consistent structure between each cell.

4.

Prompt "Can you suggest some clearer colours and better formatting for my graphs so that my lecturer or any other future users have an easier time interpreting the represented data."

Response jist: Standardized colour schemes and formats between the graphs.
