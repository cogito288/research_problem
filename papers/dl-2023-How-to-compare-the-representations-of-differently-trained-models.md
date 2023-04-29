# How to compare the representations of differently trained models

#### Paper Info 
* Title : Relative Representations Enable Zero-Shot Latent Space Communication   
* Authors: Luca Moschella, Valentino Maiorca, Marco Fumero, Antonio Norelli, Francesco Locatello, Emanuele Rodolà
* Publication : 2023.01.21 (Acceptance at ICLR 2023)
* paper link : https://arxiv.org/abs/2209.15430

#### Page Info 
* Contributors: Bumjin Park
* 2023.04.29  

## Problem 

* **❓ General Problem**: comparison of the learned representations with same architecture and dataset, but different learning strategies.
* **✅ Solved**: the last representations of two different models are angle preserving. 
* **🤔 Unsolved**: The meaning of magnitude of a representation is unclear and the angle preserving might not holds for internal representation.
* **💡 New Problem** : More problems are about how to choose a proper anchors to make relative representations and how to analyze the angles of learned representations as high dimensional representation can drastically lied on the manifold.  

## Summary 

Representation of a deep neural network is complex and is believed to impractical to directly compare two learned representations. The authors found that the angles between class centroids are maintained even though the learning methods are different. Based on the observation, the authors proposed relative representation of a absolute representation using anchors, which are randomly selected in the paper. The authors showed that relative position of a model can have similar performance with the absolute representation with NLP word representation datasets (Word2Vec and FastText) and image classification datasets (MNIST, Fashion-MNIST, CIFAR10 and CIFAR100). In addition, the authors stitched different model architectures to show that relative position can be used to communicate latent representations. 


## Discussion

The solved problem is that relative position of the representations can be leveraged to the communication of differently learned representations. This solution makes another problem, **the meaning of magnitudes of representations**.  The magnitude is removed if we only consider the angle perspective. The authors show that angles are meaningful for class-specific visualization and the individual samples are not considered properly. 
