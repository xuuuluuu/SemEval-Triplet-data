
# Aspect Sentiment Triplet Extraction Task
[ACL 2021] [Learning Span-Level Interactions for Aspect Sentiment Triplet Extraction (In ACL 2021)](https://aclanthology.org/2021.acl-long.367/)

- Please refer to this **[site](https://github.com/chiayewken/Span-ASTE)** for source code.

[EMNLP 2020] [Position-Aware Tagging for Aspect Sentiment Triplet Extraction (In EMNLP 2020)](https://arxiv.org/abs/2010.02609)

- Please refer to this **[site](https://github.com/xuuuluuu/Position-Aware-Tagging-for-ASTE)** for source code.

[AAAI 2020] [Knowing What, How and Why: A Near Complete Solution for Aspect-based Sentiment Analysis (In AAAI 2020)](https://arxiv.org/pdf/1911.01616.pdf)




# Task Description
Aspect Sentiment Triplet Extraction (ASTE) is the task of extracting the triplets of target entities, their associated sentiment, and opinion spans explaining the reason for the sentiment. This task is **firstly** proposed by (Peng et al., 2020) in the paper publised in AAAI 2020, [Knowing What, How and Why: A Near Complete Solution for Aspect-based Sentiment Analysis (In AAAI 2020)](https://arxiv.org/pdf/1911.01616.pdf)

For Example:

Given the sentence:

**The screen is very large and crystal clear with amazing colors and resolution .**

The objective of the Aspect Sentiment Triplet Extraction (ASTE) task is to predict the triplets:

**[('screen', 'large', 'Positive'), ('screen', 'clear', 'Positive'), ('colors', 'amazing', 'Positive'), ('resolution', 'amazing', 'Positive')]**
 
where a triplet consists of (target, opinion, sentiment).



# Data Description
The files in the **ASTE-Data-V2-EMNLP2020** folder are the refined data. We remove triplets that have conflicting sentiments (by SemEval) in both training, validation and test sets and also append the gold triplets at the end of each sentence to ease the triplet evaluation. We also remove the tagged sentences from the the previous ASTE-Data-V1 data released in AAAI-2020, as the tagging format results in incomplete aspect sentiment triplets. 

The data has the following format: 

> sentence####[(target position, opinion position, sentiment)]

If there are multiple triplets in the same sentence:

> sentence####[(target position, opinion position, sentiment), ..., (target position, opinion position, sentiment)]

For example:

> The screen is very large and crystal clear with amazing colors and resolution .####[([1], [4], 'POS'), ([1], [7], 'POS'), ([10], [9], 'POS'), ([12], [9], 'POS')]



# Acknowledgements
Our datasets originate from SemEval Challenges ([Pontiki 2014](https://aclanthology.org/S14-2004/); [2015](https://doi.org/10.18653/v1/S15-2082); [2016](https://aclanthology.org/S16-1002/)). The annotation (opinion label) is derived from ([Fan et al. 2019](https://aclanthology.org/N19-1259/)), where they already annotated opinion terms. 
