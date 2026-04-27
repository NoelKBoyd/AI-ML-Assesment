# Artificial Intelligence and Machine Learning

An end-to-end machine learning workflow for analysing and predicting road collisions in Sheffield, built as part of the AIML1 module assessment at Sheffield Hallam University.

## Prerequisites

Before you begin, make sure you have the following installed:

- [Python 3.12](https://www.python.org/downloads/release/python-3120/) — **other versions are not supported** (TensorFlow requires Python 3.12 or below)
- [VS Code](https://code.visualstudio.com/) with the **Python** and **Jupyter** extensions installed
- [Git](https://git-scm.com/)

## Setup Guide

### 1. Clone the repository

```bash
git clone <your-repo-url>
```

### 2. Create a virtual environment using Python 3.12

```bash
py -3.12 -m venv venv
```

### 3. Activate the virtual environment

**Windows:**

```bash
venv\Scripts\activate
```

**Mac/Linux:**

```bash
source venv/bin/activate
```

You should see `(venv)` appear at the start of your terminal prompt.

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

## AI Prompts used:

1.

Prompt "How can I carry across my pre-processed data in C1 to C2 so that the dataframe is still defined in C2"

Response: Jupyter Notebooks run in completely isolated memory environments called kernels. Save the data at the end of Criterion 1 and Load the data at the start of Criterion 2.

Code:

df.to_csv("../data/Preprocessed_Traffic_Data.csv", index=False) #save data

df = pd.read_csv("../data/Preprocessed_Traffic_Data.csv", low_memory=False) #load data

2.

Prompt "Can you suggest improvements to the analysis sections of my markdown to increase the readability and depth, do not change my analysis verdicts but make improvements"

Response jist: improved a few cells of my markdown just to make it clearer and a bit more professional / concise as I do tend to ramble in my explanations as well as improving the use of specific terminology.
