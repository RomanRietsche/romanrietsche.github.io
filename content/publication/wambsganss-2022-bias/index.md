---
title: 'Bias at a Second Glance: A Deep Dive into Bias for German Educational Peer-Review
  Data Modeling'
authors:
- Thiemo Wambsganss
- Vinitra Swamy
- Roman Rietsche
- Tanja Käser
date: '2022-01-01'
publishDate: '2025-01-21T14:54:44.235605Z'
publication_types:
- paper-conference
publication: '*Proceedings of the 29th International Conference on Computational Linguistics
  (COLING) 2022*'
abstract: Natural Language Processing (NLP) has become increasingly utilized to provide
  adaptivity in educational applications. However, recent research has highlighted
  a variety of biases in pre-trained language models. While existing studies investigate
  bias in different domains, they are limited in addressing fine-grained analysis
  on educational and multilingual corpora. In this work, we analyze bias across text
  and through multiple architectures on a corpus of 9,165 German peer-reviews collected
  from university students over five years. Notably, our corpus includes labels such
  as helpfulness, quality, and critical aspect ratings from the peer-review recipient
  as well as demographic attributes. We conduct a Word Embedding Association Test
  (WEAT) analysis on (1) our collected corpus in connection with the clustered labels,
  (2) the most common pre-trained German language models (T5, BERT, and GPT-2) and
  GloVe embeddings, and (3) the language models after fine-tuning on our collected
  data-set. In contrast to our initial expectations, we found that our collected corpus
  does not reveal many biases in the co-occurrence analysis or in the GloVe embeddings.
  However, the pre-trained German language models find substantial conceptual, racial,
  and gender bias and have significant changes in bias across conceptual and racial
  axes during fine-tuning on the peer-review data. With our research, we aim to contribute
  to the fourth UN sustainability goal (quality education) with a novel dataset, an
  understanding of biases in natural language education data, and the potential harms
  of not counteracting biases in language models for educational tasks.
tags:
- /unread
projects:
- LOOM
---
