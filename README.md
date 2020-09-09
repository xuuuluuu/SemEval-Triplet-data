# Knowing What, How and Why: A Near Complete Solution for Aspect-based Sentiment Analysis

AAAI-20 (or AAAI 2020), AAAI Conference on Artificial Intelligence

Knowing What, How and Why: A Near Complete Solution for Aspect-based
Sentiment Analysis

https://arxiv.org/pdf/1911.01616.pdf

# UPDATE on 9 Sep 2020
For the example mentioned in the paper:

The best thing about this laptop is the price along with some of the newer features .

The=O best=O thing=O about=O this=O laptop=O is=O the=O price=T-POS along=O with=O some=O of=O the=O newer=O features=TT-POS .=O

The=O best=S thing=O about=O this=O laptop=O is=O the=O price=O along=O with=O some=O of=O the=O newer=SS features=O .=O

The example consists of two target and two opinion terms, the targets are ‘price’ and ‘features’, the opinion terms are ‘best’ and ‘newer’. Note that ‘T-POS’ and ‘TT-POS’ are used for indicating different targets, and ‘S’ and ‘SS’ are used for indicating different opinion terms. Although the current data format is convenient for aspect term or opinion term extraction, there are few special cases when a few aspects shared the same opinion term, which make it hard for triplet evaluation. For sentiment triplet evaluation, we separately release the gold triplets that include all annotated triplets in the sentences. 
