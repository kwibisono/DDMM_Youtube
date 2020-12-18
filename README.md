# DDMM_Youtube

## About the project
Everyday a vast amount of information is created; and in this dynamically changing world, it is becoming increasingly difficult to pick out important information. To extract and understand information at a more digestible level, researchers have been applying clustering methods to various types of domains. These methods work effectively when the target data is static or accumulates slowly. But in fast-evolving domains such as news and online videos, clustering should be conducted dynamically. In addition, data originating from those domains tend to have limited amount of information, since there is less time for data accumulation. This introduces the need for the clustering methods to be able to deal with short texts, which are inherently sparse.

To deal with the aforementioned issues, we refer to the work of Duan et. al (2018) in which they combine the ideas of Dynamic Topic Models (DTMs), which cluster dynamically, and Dirichlet-Multinomial Mixture Models (DMMs), which cluster short text, thus resulting in a model called the Dynamic Dirichlet-Multinomial Mixture Model (DDMM). We derive and implement a collapsed Gibbs sampler for posterior inference of the model, apply it to the Trending YouTube Video Statistics dataset available on Kaggle, and subsequently conduct quantitative and qualitative analyses of the resulting clusters. We find that a slight modification of the original DDMM algorithm leads to a significant model improvement.

For more details please check DDMM_for_Short_Texts.pdf

## Dataset
Download the data from: Trending YouTube Video Statistics from https://www.kaggle.com/datasnaek/youtube-new
- Experiments were conducted on the US dataset

## Preprocessing
Run the commands in preprocessing/preprocessing.ipynb on the downloaded dataset.

## Training
Run any of the desired models notebook files in the model directory.
- Latent Dirichlet Allocation (LDA.ipynb) \[Blei et al., 2003\]
- Dynamic Topic Model (DTM.ipynb) \[Blei and Lafferty, 2006\]
- Dirichlet-Multinomial Mixture Model (DMM.ipynb) \[Yin and Wang, 2014\]
- Dynamic Dirichlet-Multinomial Mixture Model (DDMM.ipynb) \[Duan and Li, 2018\]
- Modified Dynamic Dirichlet-Multinomial Mixture Model (MDDMM.ipynb) \[Nishimura and Wibisono (Our Model), 2020\]

## Evaluation and Analysis
Except for the LDA model, all evaluation and analysis related scripts and included in "eval_analysis/evaluation and analysis.ipynb".
The evaluation and analysis for LDA can be conducted in the LDA model file.
