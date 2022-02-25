# HierarchicalABSA
Code for FiQA ABSA task using hierarchical structured language models (BERT/RoBERTa)

# Instructions:

The code is a ready to run jupyer notebook ("trainer.ipynb") which requires sufficient GPU power. First the code sections "Modules" and "Data Handler" should be runned before any of the ABSA models are runned. For the hierarchical models the model higher in the hierarchy (level 1 before level 2, level 2 before polarity) should be runned first in order to pass on predictions or model output. Each sub task is divided by (sub)headers in the notebook to easily run relevant parts of code.

# Data:

Data comes from the FiQA challenge (https://sites.google.com/view/fiqa/home) but is also attached in the data folder. It consists of Train data (1111 observations) and test data (192 observations).


