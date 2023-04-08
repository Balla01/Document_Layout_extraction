## DOCUMENT LAYOUT EXTRACTION
I have referred few papers regarding the document Layout extraction and found the LayoutLM model as the ideal one.
With the reference of LayoutLM algorithm. I have fine-tune the LayoutLM model weights and parameters by training with the given data set

# introduction

UNILM (Unified pre-trained Language Model) is a pre-trained transformer-based language model architecture. It aims to unify the pre-training of various types of natural language processing (NLP) tasks, such as language modeling, machine translation, and text summarization, into a single model. UNILM achieves this by using a multi-stage training process that gradually adds more complex NLP tasks to the pre-training objective.
LayoutLM is an extension of UNILM that is specifically designed for document layout analysis, which is the process of extracting structured information from unstructured documents. LayoutLM is pre-trained on a large corpus of scanned documents and can be fine-tuned on various downstream tasks, such as information extraction and classification.
# make sure that data is stored at the currect path, i have created the "data" file and stored the testing_data and training_data


### Steps to implement in colab note book
o	Open google drive
o	Save the ‘data’ file into the drive
o	Open the extract.ipynb file in colab
o	Mount the drive 
o	Start executing the code cell one by one
###	Important note:
o	Make sure that you have modify the paths of training and testing accordingly 
o	Please make sure you are running the code in the colab note book only

# make sure that all the packages in requirements.txt are installed
# download the pretrained models from github
! rm -r unilm
! git clone -b remove_torch_save https://github.com/NielsRogge/unilm.git
! cd unilm/layoutlm
! pip install unilm/layoutlm
! git clone https://github.com/huggingface/transformers.git
! cd transformers
! pip install ./transformers

# setup the data directory and start executing the python bloks 

## please do refer to the documentation ("LayoutML.doc") file for the more details related to algoritham
