# UNLOCKING THE SECRETS OF SPACE BIOLOGY WITH NASA OSDR DATASET

## HIGH-LEVEL SUMMARY
This project's goal is a curation of the NASA OSDR dataset to make it a more accessible, easy-to-use database for developing foundational models. We aim to make it available on Huggingface which is a very popular machine learning platform that enables researchers to apply a vast amount of Natural Language Processing models and improve the representation learning of RNA sequences. In some recent works such as RNABERT and RNA-FM, we see a great desire and need for learning better RNA representations to excel the performance on multiple tasks such as Structural Alignment, clustering, Secondary Structure Prediction, etc. Application of such foundational models on unseen datasets such as NASA OSDR can enrich it with more features and enable better analysis. On the other hand, the multimodality of this dataset could allow cross-organism studies.

## PROJECT DEMO
[presentation](https://docs.google.com/presentation/d/118ybbGZul9O8fYYm7I-i6I1FOm2T34Qf6EHuuu4ZHEY/edit?usp=sharing)

## FINAL PROJECT
[data preparation repo](https://github.com/AnzorGozalishvili/NASA_ODSR_DATA)

## PROJECT DETAILS
Our project is all about dataset curation. We aim to create a Huggingface dataset for NASA OSDR which enables scientists to easily retrieve and explore the entire dataset in several lines of Python code.

The choice of the Huggingface platform is caused by its popularity and simplicity. There are vast amounts of NLP datasets and models and it creates a competitive atmosphere between scientists to beat different NLP task leaderboards which in itself helps the development and application of such new models and architectures. Because of the high similarity of RNA sequences and natural language texts, there are many applications of NLP models in biology, but it's hard to find those models and datasets on that platform.

We have explored the NASA_OSDR dataset on the GeneLab website and identified some issues:

- cross-experimental data exploration
- missing visualizations
- many unstructured textual information in table columns
- downloading of all experiments is manual work
- hard to explore aggregated tables of assays and samples
- no preprocessed data for machine learning model training

Based on that we decided to retrieve experiment files, tables, and RNA sequences and merge them into a large feature-rich tabular dataset where cross-experimental analysis can be made.

About the application of existing foundational models such as RNABERT and RNA-FM, we are interested first in enriching the given dataset by generating RNA sequence embeddings and also making structure and function-related predictions by utilizing fine-tuned RNA-FM models on other datasets.

Having embeddings stored in a dataset repository is a very convenient way to reduce the required resources for foundational model inferences which usually require more computational resources. It will become easy to apply lightweight models such as logistic regression to learn some downstream tasks and even perform various clustering analyses. RNABERT embeddings can also be used for structural alignments and gene-identifying reference genes for given RNA sequences much faster and with quite a good accuracy as the paper authors claim.

One of the ideas we got is to identify "Space-Born RNA" sequences from the NASA OSDR dataset. This can be done by analyzing RNAs in their embedding space using different unsupervised learning approaches. The basic idea is that the environmental changes in space might require synthesizing different proteins in living organisms and therefore single cell RNA sequences must contain that information. Such kind of analysis can be definitely done on the NASA OSDR dataset since we have organisms in space vs on Earth.

In the limited time given in this competition, we tried to learn more about the problem, its importance, and its applications and we think that the curation of such a dataset must have a significant improved in biology in terms of high availability of quality datasets and models and rising the competition by bringing biology problems into ML world.

## USE OF ARTIFICIAL INTELLIGENCE
We are going to utilize openly available models such as RNABERT and RNA-FM to calculate RNA embeddings and perform clusterization to better explore given datasets. Also, we could pre-train such models on the NASA OSDR dataset from scratch or define some downstream tasks and fine-tune existing pre-trained foundational models on it.

## SPACE AGENCY DATA
[aws OSDR dataset](https://registry.opendata.aws/nasa-osdr/#:~:text=OSDR%20introduces%20access%20to%20data,AWS%20Open%20Data%20Registry%20page.)

## REFERENCES
[RNABERT repo](https://github.com/mana438/RNABERT)
[RNA-FM repo](https://github.com/ml4bio/RNA-FM)
[RNABERT paper](https://academic.oup.com/nargab/article/4/1/lqac012/6534363)
[RNA-FM paper](https://arxiv.org/abs/2204.00300)
