========================

Offensive Language Identification Dataset (OLID)
v 1.0: March 15 2018
https://scholar.harvard.edu/malmasi/olid

========================

1) DATA DESCRIPTION

This is the README file for OLID described in: https://arxiv.org/abs/1902.09666

OLID contains 14,100 annotate tweets. 
It has been used as the official dataset for OffensEval: Identifying and Categorizing Offensive Language in Social Media (SemEval 2019 - Task 6): https://competitions.codalab.org/competitions/20011

The files included are: 

- olid-training-v1.tsv contains 13,240 annotated tweets. 
- test_IN.csv contains the test set instances of level a.
- test_IN_gold.csv contains the gold labels and IDs of the instances in test set layer a.

The dataset was annotated using crowdsourcing. 
The gold labels were assigned taking the agreement of three annotators into consideration. 
No correction has been carried out on the crowdsourcing annotations. 

Twitter user mentions were substituted by @USER and URLs have been substitute by URL.

OLID is annotated using a hierarchical annotation. Each instance contains up to 3 labels each corresponding to one of the following levels:

- task A: Offensive language identification:
  (NOT) Not Offensive - This post does not contain offense or profanity.
  (OFF) Offensive - This post contains offensive language or a targeted (veiled or direct) offense

- task B: Automatic categorization of offense types;
- task C: Offense target identification.	

In our annotation, we label a post as offensive (OFF) if it contains any form of non-acceptable language (profanity) or a targeted offense, which can be veiled or direct. 


2) TASK A: Offensive or not
we are interested in the identification of offensive posts and posts containing any form of (untargeted) profanity. 
In this task there are 2 categories in which the tweet could be classified -
(NOT) Not Offensive - This post does not contain offense or profanity.  Non-offensive posts do not include any form of offense or profanity.
(OFF)Offensive - This post contains offensive language or a targeted (veiled or direct) offense.  In our annotation, we label a post as offensive if it  contains any form of non-acceptable language (profanity) or a targeted offense which can be veiled or direct. To sum up this category includes insults, threats, and posts containing profane language and swear words.


3) CITING THE DATASET

If you use this dataset we kindly ask you to include a reference to the paper below. 

@inproceedings{zampierietal2019, 
title={{Predicting the Type and Target of Offensive Posts in Social Media}}, 
author={Zampieri, Marcos and Malmasi, Shervin and Nakov, Preslav and Rosenthal, Sara and Farra, Noura and Kumar, Ritesh}, 
booktitle={Proceedings of NAACL}, 
year={2019}, 
} 

The paper will be presented at NAACL and the pre-print is available on arXiv.org: https://arxiv.org/abs/1902.09666

If you would like to refer to the OffensEval competition, here is the bib entry to the report:

@inproceedings{offenseval,
title={{SemEval-2019 Task 6: Identifying and Categorizing Offensive Language in Social Media (OffensEval)}},
author={Zampieri, Marcos and Malmasi, Shervin and Nakov, Preslav and Rosenthal, Sara and Farra, Noura and Kumar, Ritesh},
booktitle={Proceedings of The 13th International Workshop on Semantic Evaluation (SemEval)},
year={2019}
}
