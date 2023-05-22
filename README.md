Turkish NER dataset from Wikipedia sentences. 20.000 sentences are sampled and re-annotated from [Kuzgunlar NER dataset](https://data.mendeley.com/datasets/cdcztymf4k/1).


Data split:

- 18.000 train
- 1000 test
- 1000 dev

Labels:

- CARDINAL
- DATE
- EVENT
- FAC
- GPE
- LANGUAGE
- LAW
- LOC
- MONEY
- NORP
- ORDINAL
- ORG
- PERCENT
- PERSON
- PRODUCT
- QUANTITY
- TIME
- TITLE
- WORK_OF_ART

Dataset is in **conll** format. Here's an example from the sample for you:

```
Çekimler	O
5	B-DATE
Temmuz	I-DATE
2005	I-DATE
tarihinde	O
Reebok	B-FAC
Stadyum	I-FAC
,	O
Bolton	B-GPE
,	O
İngiltere'de	B-GPE
yapılmıştır	O
.	O
```
or even better:

![ingiltere](https://github.com/turkish-nlp-suite/Turkish-Wiki-NER-Dataset/assets/8277232/f130a1e9-a3e7-40b9-8204-4917d89607b8)


Annotations are done by [Co-one](https://co-one.co/). Many thanks to them for their contributions. This dataset is also used in our brand new spaCy Turkish packages.

This work is supported by Google Developer Experts Program.
Part of Duygu 2022 Fall-Winter collection, "Turkish NLP with Duygu"/ "Duygu'yla Türkçe NLP". All rights reserved.
