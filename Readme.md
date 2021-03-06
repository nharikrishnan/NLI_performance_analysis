# Performance Analysis of methodologies for natural language interpretation
In this project the performance of traditional NLP methods, machine learning models and ensemble approaches in natural language interpretation was analyzed by understanding the semantic equivalence of pairs of sentences/questions and classifying them as duplicate or not duplicate. The best combination of feature extraction technique and Machine learning model with the best parameter is also found.<br>
We have tested the methods using question pair data set and Microsoft paraphrase data set.

### Methods
<ul><li><b> Traditional NLP</b> (methods based on similarity)</li>
  <ul>
    <li>Sim Hash</li>
    <li>NER similarity</li>
    <li>Cosine Similarity</li>
  </ul>
  <li> <b>ML and ensemble models</b></li>
  <ul>
    <li> Logistic regression </li>
    <li> SVM </li>
    <li> Random Forest</li>
    <li> XGB Classifier</li>
    <li> Adaboost Classifier </li>
    <li> Voting Classifier </li>
  </ul>
  <li><b>Deep Learning models</b></li>
  <ul>
    <li>Siamese LSTM</li>
    <li>Siamese CNN</li>
    <li>Siamese GRU</li>
    <li>Enhanced LSTM</li>
    <li>hybrid models</li>
  </ul>
</ul>
<p><img src="Architecture.png" style="float:center" alt="drawing" width="500"/></p>


## Getting Started
The models developed for this project can be used for any similar tasks, there are many functions created for this project which can be reused for the same purpose.

### Prerequisites
Python version 3.7.7 was used for development.<br>
Python Packages required can be found in <i>'requirement.txt'</i><br>
The packages can be installed using the command:
```
pip install 'package_name'
```
#### Word embedding
Glove.6b.50d.txt word embedding file is used assigning weights in embedding layer for all deep learning tasks.
1. Instructions to download the word embedding file is given inside word embedding folder, download the word embedding file fllowin the instruction and keep the glove.6b.50d.txt file inside the word embedding folder.

### Folder structure

The <b>data</b> folder contains both quora and msr csv files. <br> <br>
<b>Functions</b> folder contains all the user defined function used in the project <br><br>
<b>Models</b> folder contains both deep learning and machine learning models. The execution of these models can be found in the root folder as .ipynb files.<br><br>
Parameter tuning for deep learning and machine learning models can be found in the <b>parameter tuning</b> folder

### Executing the models ipynb for testing
<ol> <li>Clone the repository, and place the GLove word vector file in the word embedding directory</li>
    <li>If the structure of the repository is maintained all models can be used and also all notebooks present the root directory can be tested
    <li> To generate the predictions csv for each model, run the .py files with corresponding name</li>
    <ul>For example


```
py machine_learning.py
```
this will generate output for all the machine learning models, similarly use deeplearning.py for deeplearning models and NLP_sim.py for similarity based NLP methods
And repeat
</ol>

### output
Output for each method generated inside the result Folder
<ul><li>All the outputs for Quora question pair data are generated inside the quora folder inside results folder</li>
    <li>All the outputs for MSR Paraphrase data are generated inside the MSR folder inside results folder</li> </ul>
