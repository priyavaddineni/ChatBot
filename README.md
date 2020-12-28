# ChatBot

A Chatbot implemented using sequence to sequence model.

### **Recommended Reading**


1.   [Sequence to Sequence Learning with Neural Networks](https://arxiv.org/abs/1409.3215)
2.   [A Neural Conversational Model](https://arxiv.org/abs/1506.05869)

### Prerequisites

jupyterlab<br>
requests<br>
matplotlib<br>
nltk<br>
numpy<br>
beautifulsoup4<br>
sklearn<br>
torch<br>
regex<br>
json<br>
bleu

We need to make sure that torch cuda version and NVIDIA cuda verison are same

### Data

Data required is available in `data` folder but if you need to generate it on your own, run `extract_data.ipynb`. This will generate two main files which includes `joeyConversations.json` and `TVConversations.json`. After generation, `TVConversations.json` should be combined with Cornell conversations data which is available in `data` folder for training first phase. Combined data is also available in data folder.

###  Model

Detailed explanation of implementation is available at `chatbot.ipynb`. Run this file using the data generated above and see results. This file saves the model for each training phase, which is pretty large. Saved file can be used anytime later for evaluation. You can use different set of parameters for optimization, but what i have in my code seems to be best for current data.
