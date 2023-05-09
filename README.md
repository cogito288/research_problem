# How to read a paper & How to select a research topic
A message from a professor... 

✅ tl;dr: It is important to know what is solved and what is unsolved.
- Summarize the limitations of the existing methods.
- Critically think whether the problem is really solved or partially solved (or it is a marginal improvement). Ask yourself if the proposed algorithm fundamentally solves the given problem and if it does, think about which aspect of the algorithm makes the problem solved.
- Check what would be the remaining problem. The remaining problem can be a chance for you for a research topic.
- As "guru"s clearly write what is the problem and which part is solved, it will be helpful to refer to such papers to collect the current problems.
- It is more important to know (or to collect) the problems, than studying existing methods.
- Consider the research topic to be algorithmic things we can do well, not too big topics
- Check out lots of tutorials 

# Research Problems

This is repository is collect research problems regarding how we can edit the models. Regarding editing, we can categorize into 
* Concept/Neuron/Unit Matching
* Editing/Correcting/Perturbation w/ re-training
* Inference editing = Editing/Correcting/Perturbation w/o. re-training

## Survey Papers
| Venue | Year | Title | Affiliation | Link | Source |
| :---: | :---: | :--- | :---: | :---: | :---: |
| TACL | 2022 | Neuron-level interpretation of deep nlp models: A survey | | [[paper]](https://direct.mit.edu/tacl/article-abstract/doi/10.1162/tacl_a_00519/113852) |  |

## Concept/Neuron/Unit Matching/Alignment
| Venue | Year | Title | Affiliation | Link | Source |
| :---: | :---: | :--- | :---: | :---: | :---: |
| ECCV | 2020 | Rewriting a Deep Generative Model | MIT | [[paper]](http://rewriting.csail.mit.edu/) | [[code]](https://github.com/davidbau/rewriting) |
| PNAS | 2020 | Understanding the Role of Individual Units in a Deep Neural Network | MIT | [[paper]](http://dissect.csail.mit.edu/) | [[code]](https://github.com/davidbau/dissect) |
| ICCV | 2019 | Seeing what a GAN Cannot Generate | MIT | [[paper]](http://gandissect.csail.mit.edu/papers/Seeing_What_a_GAN_Cannot_Generate.pdf) | [[code]](https://github.com/davidbau/ganseeing) |
| ICLR | 2019 | GAN dissection | MIT | [[paper]](http://gandissect.csail.mit.edu/) | [[code]](https://github.com/CSAILVision/gandissect) |
| arXiv | 2022 | `CRP` From" Where" to" What": Towards Human-Understandable Explanations through Concept Relevance Propagation | Fraunhofer HHI | [[paper]](https://arxiv.org/abs/2206.03208) | [[code]](https://github.com/rachtibat/zennit-crp) |
| CVPR | 2022 | HINT: Hierarchical Neuron Concept Explainer | HKU | [[paper]](http://openaccess.thecvf.com/content/CVPR2022/html/Wang_HINT_Hierarchical_Neuron_Concept_Explainer_CVPR_2022_paper.html) | [[code]]() |
| ICLR | 2022 | Attention-based Interpretability with Concept Transformers | IBM | [[paper]](https://openreview.net/forum?id=kAa9eDS0RdO) | [[code]](https://github.com/IBM/concept_transformer) |
| ECCV | 2022 | Making Heads or Tails: Towards Semantically Consistent Visual Counterfactuals | Meta AI | [[paper]](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136720260.pdf) | [[code]](https://github.com/facebookresearch/visual-counterfactuals) |
| arXiv | 2022 | Neural activation patterns (NAPs): Visual explainability of learned concepts | Ulm Univ. | [[paper]](https://arxiv.org/abs/2206.10611) |  |
| ACL | 2022 | Knowledge Neurons in Pretrained Transformers | Microsoft | [[paper]](https://arxiv.org/pdf/2104.08696.pdf) | [[code]](https://github.com/hunter-ddm/knowledge-neurons) |
| arXiv | 2022 | Measuring Causal Effects of Data Statistics on Language Model's ‘Factual' Predictions | | [[paper]](https://arxiv.org/abs/2207.14251) | [[weight]](https://huggingface.co/yanaiela/roberta-base-epoch_83) |
| ECCV | 2022 | Compositional visual generation with composable diffusion models | UIUC & MIT | [[paper]](https://link.springer.com/chapter/10.1007/978-3-031-19790-1_26) | [[code]](https://github.com/energy-based-model/Compositional-Visual-Generation-with-Composable-Diffusion-Models-PyTorch) |
| arXiv | 2021 | Do language models have beliefs? methods for detecting, updating, and visualizing model beliefs | | [[paper]](https://arxiv.org/abs/2111.13654) | [[code]](https://github.com/peterbhase/SLAG-Belief-Updating) |
| NLPCC | 2022 | Kformer: Knowledge injection in transformer feed-forward layers | | [[paper]](https://link.springer.com/chapter/10.1007/978-3-031-17120-8_11) | [[code]](https://github.com/zjunlp/Kformer) |
| EMNLP | 2022 | Finding Skill Neurons in Pre-trained Transformer-based Language Models | Tsinghua | [[paper]](https://arxiv.org/abs/2211.07349) | [[code]](https://github.com/THU-KEG/Skill-Neuron) |
| EMNLP | 2022 | You Are My Type! Type Embeddings for Pre-trained Language Models | EURECOM | [[paper]](https://aclanthology.org/2022.findings-emnlp.336.pdf) | [[code]](https://github.com/MhmdSaiid/TypeEmbedding) |


## Editing/Correcting/Perturbation w/ re-training
You can refer to `editing` directories in papers.

## Inference editing
Editing/Correcting/Perturbation w/o. re-training. 

### Editing - needed to separated into re-training and inference editing
Sure! Here's the markdown table for the list of papers you provided:

| Venue | Year | Title | Affiliation | Link | Source |
| :---: | :---: | :--- | :---: | :---: | :---: |
| arXiv | 2023  | [`DreamBooth`](papers/editing/2023_dreambooth.md): Fine Tuning Text-to-Image Diffusion Models for Subject-Driven Generation | Google | [[paper]](https://arxiv.org/abs/2208.12242) | [[Official dataset]](https://github.com/google/dreambooth) <br /> [[Unofficial]](https://github.com/XavierXiao/Dreambooth-Stable-Diffusion) |
| | 2023 | Erasing Concepts from Diffusion Models | | [[paper]]( http://arxiv.org/abs/2303.07345) | [[code]]() | 
| | | Locating and Editing Factual Associations in GPT | | [[paper]](http://rome.baulab.info/) | [[code]]() |
| | | GAN Paint | | [[paper]](http://ganpaint.io/) | [[code]]() |
| | | Network Dissection | | [[paper]](http://netdissect.csail.mit.edu/) | [[code]]() |
| NeurIPS 2021 | 2021 | Editing a classifier by rewriting its prediction rules | | [[paper]](https://proceedings.neurips.cc/paper/2021/hash/c46489a2d5a9a9ecfc53b17610926ddd-Abstract.html) | [[code]]() |
| ACM CHI 2022 | 2022 | Interpretability, Then What? Editing Machine Learning Models to Reflect Human Knowledge and Values | | [[paper]](https://dl.acm.org/doi/abs/10.1145/3534678.3539074) | [[code]]() |
| | | MASS-EDITING MEMORY IN A TRANSFORMER | | [[paper]]() | [[code]]() |
| CVPR 2020 | 2020 | Counterfactual Vision and Language Learning | | [[paper]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Abbasnejad_Counterfactual_Vision_and_Language_Learning_CVPR_2020_paper.pdf) | [[code]]() |
| | | DiffEdit: Diffusion-based semantic image editing with mask guidance | | [[paper]]() | [[code]]() |
| | | Blended Diffusion for Text-driven Editing of Natural Images | | [[paper]]() | [[code]]() |
| | | Imagic: Text-Based Real Image Editing with Diffusion Models | | [[paper]]() | [[code]]() |
| | | EDICT: Accurate Text-Guided Image Editing with Diffusion Models | | [[paper]]() | [[code]]() |
| | | Muse: Text-To-Image Generation via Masked Generative Transformers | | [[paper]]() | [[code]]() |
| ICLR 2022 | 2022 | Aging with GRACE: Lifelong Model Editing with Key-Value Adaptors | | [[paper]](https://openreview.net/forum?id=ngCT1EelZk) | [[code]]() |
| arXiv | 2023 | Robustness of edited neural networks | | [[paper]](https://arxiv.org/abs/2303.00046) | [[code]]() |
| arXiv | 2023 | Editing Implicit Assumptions in Text-to-Image Diffusion Models | | [[paper]](https://arxiv.org/abs/2303.08084) | [[code]]() |
| arXiv | 2022 | Planning with Diffusion for Flexible Behavior Synthesis | | [[paper]](https://arxiv.org/abs/2205.09991) | [[code]]() |
| arXiv | 2021 | Fast model editing at scale | | [[paper]](https://arxiv.org/abs/2110.11309) | [[code]]() |
| arXiv | 2021 | Sparse interventions in language models with differentiable masking | | [[paper]]() | [[code]]() |


# Acknowledgements
* `bumjin@kaist.ac.kr` : Bumjin Park, [@fxnnxc](https://github.com/fxnnxc)
* [awesome-gnn-systems](https://github.com/chwan1016/awesome-gnn-systems) of [@chwan1016](https://github.com/chwan1016)

# TODO
- [ ] Add the number of citations and github stars using Github Actions.
- [ ] Delete affliation column Or check again affliation for the cases where it has more than one afflication.
- [ ] Sort rows based on the year.
---