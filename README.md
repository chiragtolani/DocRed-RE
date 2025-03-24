```markdown
# Project Name

A Multi-Model Approach to Relation Extraction: BERT Embeddings with XGBoost and Graph Neural Networks

## About the Project
This project focuses on Relation Extraction, comparing two major approaches: a traditional machine learning model and a graph-based neural network. We implement XGBoost as our traditional model and Graph Convolutional Networks (GCN) as our graph-based approach, utilizing the re-DOCRED dataset. For both models, the input data is pre-processed and converted into BERT embeddings to capture rich contextual features. The goal is to evaluate and compare the performance of these distinct methodologies in extracting relationships from text data.

## Built With
- [Python](https://www.python.org/)
- [Jupyter](https://jupyter.org/)
- [PyTorch](https://pytorch.org/)

## Getting Started

To get a local copy up and running, follow these steps:

### Prerequisites
- Python 3.12 or more installed
- pip (Python package manager)
- conda (optional)

### Installation

1. Create a virtual environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install the required dependencies
```bash
pip install -r requirements.txt
```

**Please note that for importing torch-cluster library, Visual C++ libraries should be already installed (Visual Studio Build Tools: You’ll need a C++ compiler, and Microsoft’s Visual Studio Build Tools is the standard choice)**

**Minimum components: MSVC C++ build tools,Windows SDK**

## Contact
- Aishwarya Kulkarni - Student ID: [11606062] - [aishwarya.kulkarni@postgrad.manchester.ac.uk]
- Vaibhav Parihar - Student ID: [11544144] - [vaibhav.parihar@postgrad.manchester.ac.uk]
- Shreya Varghese - Student ID: [11603111] - [shreya.varghese@postgrad.manchester.ac.uk]
- Chirag Tolani - Student ID: [14124054] - [chirag.tolani@postgrad.manchester.ac.uk]

## Other Remarks

Please refer to the mentioned link for the dataset utilized for this project: https://github.com/tonytan48/Re-DocRED

Due to memory restrictions, please find all the files in the following OneDrive link incase its not accessed on Blackboard:

Kindly note that the following folder and file structure of our project: https://livemanchesterac-my.sharepoint.com/:f:/g/personal/chirag_tolani_postgrad_manchester_ac_uk/EtJjqPIN0NJLjjbbMs2fYLsBx2JOqpHv15fPu3BEhnVeZA?e=nKdZe0

**requirements.txt** - This file contains all the required libraries and functions that need to installed and imported into the notebook files. Installation guide for these libraries are detailed in the Installation section
**bert_embeddings** - These are the extracted BERT embeddings that are saved during the pre-processing step for both the models
**XGB_model_and_embeddings** - This folder contains the model file saved during the training loop (.pkl file) as well as the optimal thresholds utilized to improve the XGBOOST model performance
**GCN_model_and_embeddings** - This folder contains the model file saved during the training loop (.pkl file) as well as the optimal thresholds utilized to improve the GCN model performance
**bert_with_xgboost.ipynb** - This notebook contains the preprocessing of the dataset into BERT embeddings as well as the training code for the XGBoost model
**bert_with_gcn.ipynb** - This notebook contains the preprocessing of the dataset into BERT embeddings as well as the training code for the GCN model
**xgboost_inference.ipynb** - This notebook contains the code to perform real time inference on XGBoost model and predict the relations for the provided user input
**gcn_inference.ipynb** - This notebook contains the code to perform real time inference on GCN model and predict the relations for the provided user input
**rel_info.json** - contains the relation mapping required for real time inference of both models

Please note on the same zip file, contains three main dataset files - **train_revised.json**, **test_revised.json** and **dev_revised.json** that are the training data, testing data and validation data respectively. 

We have also include a short research paper (**RE-paper-final.pdf**) detailing on the approaches applied on the dataset for relation extraction, discussion on related work, the methodology applied on both the approaches and evaluation of the performance of both approaches. The paper also provides a comparative analysis of both the models and limitations faced during the implementation phase. The paper is also uploaded on OneDrive link as well.


```