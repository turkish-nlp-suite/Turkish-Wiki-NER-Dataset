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

This dataset is available on [Huggingface](https://huggingface.co/datasets/turkish-nlp-suite/turkish-wikiNER) as well, you can use it as:

```
from datasets import load_dataset

dataset = load_dataset("turkish-nlp-suite/turkish-wikiNER")
```


Annotations are done by [Co-one](https://co-one.co/). Many thanks to them for their contributions. This dataset is also used in our brand new spaCy Turkish packages.

This work is supported by Google Developer Experts Program.
Part of Duygu 2022 Fall-Winter collection, "Turkish NLP with Duygu"/ "Duygu'yla Türkçe NLP". All rights reserved. If you'd like to use this dataset in your own work, please kindly cite [A Diverse Set of Freely Available Linguistic Resources for Turkish](https://aclanthology.org/2023.acl-long.768/) :

```
@inproceedings{altinok-2023-diverse,
    title = "A Diverse Set of Freely Available Linguistic Resources for {T}urkish",
    author = "Altinok, Duygu",
    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.acl-long.768",
    pages = "13739--13750",
    abstract = "This study presents a diverse set of freely available linguistic resources for Turkish natural language processing, including corpora, pretrained models and education material. Although Turkish is spoken by a sizeable population of over 80 million people, Turkish linguistic resources for natural language processing remain scarce. In this study, we provide corpora to allow practitioners to build their own applications and pretrained models that would assist industry researchers in creating quick prototypes. The provided corpora include named entity recognition datasets of diverse genres, including Wikipedia articles and supplement products customer reviews. In addition, crawling e-commerce and movie reviews websites, we compiled several sentiment analysis datasets of different genres. Our linguistic resources for Turkish also include pretrained spaCy language models. To the best of our knowledge, our models are the first spaCy models trained for the Turkish language. Finally, we provide various types of education material, such as video tutorials and code examples, that can support the interested audience on practicing Turkish NLP. The advantages of our linguistic resources are three-fold: they are freely available, they are first of their kind, and they are easy to use in a broad range of implementations. Along with a thorough description of the resource creation process, we also explain the position of our resources in the Turkish NLP world.",
}
```
