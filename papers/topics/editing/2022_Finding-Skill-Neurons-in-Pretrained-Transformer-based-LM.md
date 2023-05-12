📌TL;DR: **Find some special neurons in pre-trained Transformers whose activations on soft prompts are highly predictive of the task labels of inputs.**



## Problem 
* **👀 Motivation**: It remains unclear how the skills required to handle NLP tasks distribute among model parameters

* **❓ General Problem**: Are there specific neurons within pre-trained Transformers encoding task-specific skills?

* **✅ Solved**: Develop a simple and effective method to find the specific neurons, *Skill Neurons*, for classification tasks via **prompt tuning**.
    - For a binary classification task, calculate the empirical mean activation on a soft prompt token over the training set for each neuron and use it as this neuron’s baseline activation.
    - If this neuron’s activation for an input sample is higher than the baseline, regard it as predicting one label and vice versa.
    - Aggregate the prediction accuracies on the validation set of multiple soft prompts as the neuron’s predictivity score.
    - The neurons with the highest predictivity scores are identified as skill neurons.

* **🤔 Unsolved (Limitations)**:
  - The scope of the task is limited to classification.
  - It is not clear why skill neurons are generated during the pre-training process.
  - The author claims that pre-trained transformers can be analyzed more deeply using skill neurons. In fact, since skill neurons were found using only FFN, interactions with other parameters in Transformers need to be considered for more reliable analysis.

* **💡 New Problem** :
  - Why is prompt tuning helpful in finding skill neurons?
  - It is necessary to observe the characteristics of the token used as the predictive score of the skill neuron.
  - In order to find answers to the above two problems, research to understand the interaction with the attention mechanism is needed.


# Paper

### Paper Info 
* Title : Finding Skill Neurons in Pre-trained Transformer-based Language Models
* Authors: Xiaozhi Wang, Kaiyue Wen, Zhengyan Zhang, Lei Hou, Zhiyuan Liu, Juanzi Li
* Publication : 2022.11.14
* paper link : https://arxiv.org/pdf/2211.07349.pdf

### Page Info 
* Contributors: Youngju Joung
* 2023.05.11

## Summary 
* Contributions
  - Observe the existence of skill neurons, the special neurons within pre-trained Transformers, which are highly predictive for specific tasks, and develop a method to find them via prompt tuning.
* Analysis
  - Skill neurons are crucial for handling tasks and task-specific.
  - Skill Neurons are not from Word Selectivity and most likely generated in pre-training
* Application
  - Pruning based on skill neurons generally performs comparably to vanilla prompt tuning and can achieve about 1.4 inference speedup.
