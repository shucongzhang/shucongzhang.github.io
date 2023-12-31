---
layout: archive
title: ""
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

This page categorizes papers based on their research topics. For a "clean" list of publications, please to [my Goole Scholar](https://scholar.google.com/citations?hl=en&user=ZK1dMoYAAAAJ&view_op=list_works) 

<h1>The (Un)usefulness of Attention Mechanisms for Speech Recognition</h1>
<hr/>

Although attention-based models, especially Transformer variants, have been shown to provide outstanding performance in automatic speech recognition (ASR), it is questionable whether attention is necessary for ASR. The reasoning is straightforward: when recognizing a current word, humans do not rely on words spoken tens of seconds later by the speaker, yet attention mechanisms do. Currently, our linear models have outperformed both Branchformer and Conformer models, achieving state-of-the-art (SOTA) ASR results across five different languages and three distinct acoustic conditions. 

1. T. Parcollet^, R. van Dalen^, **S. Zhang^**, S Bhattacharya (^ equal contribution). "[Sumformer: A Linear-Complexity Alternative to
Self-Attention for Speech Recognition](https://arxiv.org/pdf/2307.07421.pdf)" (preprint 2023. Paper to be updated soon.)
<br/>**TL;DR**: A linear alternative to self-attention reduces the VRAM usage by half and the training/inference time by up to 28%, and outperforms SOTA speech recognition models across five different languages under three different acoustic conditions. The benefits can also be generalized to speech understanding.

2. **S. Zhang**, E. Loweimi, P. Bell, S. Renals. “[On the Usefulness of Self-Attention for Automatic Speech Recognition with Transformers.](https://arxiv.org/pdf/2011.04906.pdf)” **IEEE Spoken Language Technology Workshop (SLT) 2021**
<br/>**TL;DR**: We unveil that for Transformer-based speech recognition systems, some self-attention layers can behave similarly to and can be replaced by linear layers. (Subsequent works show a similar conclusion has also been observed for SOTA speech recognition systems based on [Conformer](https://openreview.net/pdf?id=AvcfxqRy4Y) and [Branchformer](https://arxiv.org/pdf/2207.02971.pdf).)

3. **S. Zhang**, E. Loweimi, P. Bell, S. Renals. “[Stochastic Attention Head Removal: A Simple and Effective Method for Improving Automatic Speech Recognition with Transformers.](https://arxiv.org/pdf/2011.04004v1.pdf)” **INTERSPEECH 2021**
<br/>**TL;DR**: We show that not all attention heads are necessary in Transformer-based speech recognition systems. Removing attention heads randomly during training can improve the performance of SOTA Transformer and Conformer speech recognition models. 

4. **S. Zhang**, E. Loweimi, P. Bell, S. Renals. “[Windowed attention mechanisms for speech recognition.](https://www.pure.ed.ac.uk/ws/portalfiles/portal/80931064/WINDOWED_ATTENTION_MECHANISMS_FOR_SPEECH_RECOGNITION.pdf)” **ICASSP 2019**
<br/>**TL;DR**: For the attentional encoder-decoder speech recognition system, we demonstrate restricting the attention mechanism to attend to a window of input frames with trained window length and shift will improve the accuracy and reduce the time complexity. 

5. **S. Zhang**, E. Loweimi, Y. Xu, P. Bell, S. Renals. “[Trainable Dynamic Subsampling for End-to-End Speech Recognition.](https://www.isca-speech.org/archive/pdfs/interspeech_2019/zhang19d_interspeech.pdf)” **INTERSPEECH 2019**
<br/>**TL;DR**: We demonstrate that a fully trainable input sequence subsampling strategy for attention-based ASR models outperforms conventional subsampling methods with fixed sampling rates..

<h1>Self-supervised Learning for Speech Processing</h1>
<hr/>

Self-supervised learning (SSL) typically requires extremely large amounts of resources, which can prevent the advancement of this area. Additionally, training such models often results in a large carbon footprint. We aim to make the training of SSL more accessible and environmentally friendly. Currently, we speed up the training of SOTA SSL models up to 3.7x and reduce the GPU requirement from A100 GPUs to RTX 3090 GPUs.

1. T. Parcollet, H. Nguyen, S. Evain, M. Zanon Boito, A. Pupier, S. Mdhaffar, H. Le, S. Alisamir, N. Tomashenko, M. Dinarelli, **S. Zhang**, A. Allauzen, M. Coavoux, Y. Esteve, M. Rouvier, J. Goulian, B. Lecouteux, F. Portet, S. Rossato, F. Ringeval, D. Schwab, L. Besacier. "[LeBenchmark 2.0: a Standardized, Replicable and Enhanced Framework for
Self-supervised Representations of French Speech](https://arxiv.org/pdf/2309.05472.pdf)" (preprint 2023. Paper to be updated soon. )
<br/>**TL;DR**: We conducted benchmarks and open-sourced self-supervised learning models for French speech, which encompassed data ranging from 1,000 to 14,000 hours and model sizes from 26 million to 1 billion parameters. Additionally, we explored the pre-training and fine-tuning techniques for downstream tasks and their impact on the carbon footprint.

2. T. Parcollet, **S. Zhang**, R. van Dalen, AGCP. Ramos, S. Bhattacharya. "[On the (In)Efficiency of Acoustic Feature Extractors for
Self-Supervised Speech Representation Learning](https://hal.science/hal-04116371/document)" **INTERSPEECH 2023**
<br/>**TL;DR**: We carefully design the feature extractor frontend for self-supervised speech processing models, successfully reducing the minimum hardware requirements for training state-of-the-art (SOTA) models from A100 GPUs to RTX 3090 GPUs.

<h1>Noise Robust Speech Recognition</h1>
<hr/>

We address noisy inputs from two approaches: 1. training a speech enhancement front-end to remove noise, and 2. using transfer learning to enable the ASR model to learn noise-invariant features.

1. **S. Zhang**, M. Chadwick, AGCP. Ramos, T. Parcollet, R. van Dalen, S. Bhattacharya. "[Real-Time Personalised Speech Enhancement Transformers with Dynamic
Cross-attended Speaker Representation](https://www.isca-speech.org/archive/pdfs/interspeech_2023/zhang23r_interspeech.pdf)" **INTERSPEECH 2023**
<br/>**TL;DR**: We demonstrate that the cross-attention mechanism, despite its apparent computational expense, is more effective than conventional static single-vector approaches in learning speaker representations. Consequently, speech enhancement systems based on cross-attention outperform traditional models, achieving better performance with a smaller model size, which in turn results in faster speech inference.

2. **S. Zhang**, CT. Do, R. Doddipatla, E. Loweimi, P. Bell, S. Renals. “[Train Your Classifier First: Cascade Neural Networks Training from Upper Layers to Lower Layers.](https://arxiv.org/pdf/2102.04697.pdf)” **ICASSP 2021**
<br/>**TL;DR**: We demonstrate that training neural networks layer by layer, starting from the upper layers (near the output) and progressing to the lower layers (near the input), can yield substantial and consistent performance gains for speech recognition, image classification, and language modeling tasks.

3. **S. Zhang**, CT. Do, R. Doddipatla, S. Renals. “[Learning Noise Invariant Features Through Transfer Learning for Robust End-to-End Speech Recognition.](https://www.pure.ed.ac.uk/ws/portalfiles/portal/138528386/Learning_Noise_Invariant_ZHANG_DOA24012020_AFV.pdf)” **ICASSP 2020**
<br/>**TL;DR**: We show the upper layers (near the output) of the neural-based speech recognition models are more robust to noise and thus can be used to guide the lower layers of the network to learn noise-invariant features.

4. CT. Do, **S. Zhang**, T. Hain. “[Selective Adaptation of End-to-End Speech Recognition using Hybrid CTC/Attention Architecture for Noise Robustness.](https://eurasip.org/Proceedings/Eusipco/Eusipco2020/pdfs/0000321.pdf)” **European Signal Processing Conference (EUSIPCO) 2020**
<br/>**TL;DR**: “With a constraint on computational budget, we benchmark which part of LSTM-based speech recognition systems is the most effective for noise-robust adaptation using a very limited amount data (about 2.4 minutes).”

<h1>Streaming Transformer ASR Model</h1>
<hr/>

1. M. Li, **S. Zhang**, C. Zorila, R. Doddipatla. “[Transformer-based Streaming ASR with Cumulative Attention.](https://arxiv.org/pdf/2203.05736.pdf)” **ICASSP 2022**
<br/>**TL;DR**: We enhance the performance of Transformer-based encoder-decoder streaming speech recognition systems, achieving improvements in both speed and accuracy.
