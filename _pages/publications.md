---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}


Mohan Li, **Shucong Zhang**, Catalin Zorila, and Rama Doddipatla. “Transformer-based Streaming ASR with Cumulative Attention.” ICASSP 2022
 
**Shucong Zhang**, Cong-Thanh Do, Rama Doddipatla, Erfan Loweimi, Peter Bell, and Steve Renals. “Train Your Classifier First: Cascade Neural Networks Training from Upper Layers to Lower Layers.” ICASSP 2021

**Shucong Zhang**, Erfan Loweimi, Peter Bell, and Steve Renals. “Stochastic Attention Head Removal: A Simple and Effective Method for Improving Automatic Speech Recognition with Transformers.” INTERSPEECH 2021
   
**Shucong Zhang**, Erfan Loweimi, Peter Bell, and Steve Renals. “On the Usefulness of Self-Attention for Automatic Speech Recognition with Transformers.” IEEE Spoken Language Technology Workshop (SLT) 2021
   
**Shucong Zhang**, Cong-Thanh Do, Rama Doddipatla, and Steve Renals. “Learning Noise Invariant Features Through Transfer Learning for Robust End-to-End Speech Recognition.” ICASSP 2020
   
Cong-Thanh Do, **Shucong Zhang**, and Thomas Hain. “Selective Adaptation of End-to-End Speech Recognition using Hybrid CTC/Attention Architecture for Noise Robustness.” European Signal Processing Conference (EUSIPCO) 2020

**Shucong Zhang**, Erfan Loweimi, Peter Bell, and Steve Renals. “Windowed attention mechanisms for speech recognition.” ICASSP 2019

**Shucong Zhang**, Erfan Loweimi, Yumo Xu, Peter Bell, and Steve Renals. “Trainable Dynamic Subsampling for End-to-End Speech Recognition.” INTERSPEECH 2019

