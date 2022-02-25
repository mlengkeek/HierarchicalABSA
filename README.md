# HierarchicalABSA
Code for FiQA ABSA task using hierarchical structured language models (BERT/RoBERTa)

# Instructions:

The code is a ready to run jupyer notebook ("trainer.ipynb") which requires sufficient GPU power. First the code sections "Modules" and "Data Handler" should be runned before any of the ABSA models are runned. For the hierarchical models the model higher in the hierarchy (level 1 before level 2, level 2 before polarity) should be runned first in order to pass on predictions or model output. Each sub task is divided by (sub)headers in the notebook to easily run relevant parts of code. In order to choose to run BERT-base/BERT-TRC2/RoBERTa uncommment the associated: tokenizer, model (in the model_init), and hyperparameters within a cell, make sure to use the same model type for hierarchical following model. The pretrained language models should be put in the "models/language_models/XXX" directory where XXX denotes RoBERTa or TRC2. The language model for TRC2 can be found on https://github.com/ProsusAI/finBERT and the language model for RoBERTa on https://huggingface.co/roberta-base/tree/main. The "pytorch_model.bin" placeholder within "models/language_models/XXX" should be replaced by the associated language model.

# Data:

Data comes from the FiQA challenge (https://sites.google.com/view/fiqa/home) but is also attached in the data folder. It consists of Train data (1111 observations) and test data (192 observations).

# Related work and code:

Araci, D. (2019). Finbert: Financial sentiment analysis with pre-trained language models. arXiv preprint arXiv:1908.10063. (https://github.com/ProsusAI/finBERT)

Yang, H., Zeng, B., Yang, J., Song, Y., & Xu, R. (2021). A multi-task learning model for chinese-oriented aspect polarity classification and aspect term extraction. Neurocomputing, 419, 344-356. (https://github.com/yangheng95/LCF-ATEPC)



