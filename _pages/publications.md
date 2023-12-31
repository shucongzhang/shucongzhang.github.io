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

This page includes a TL;DR for each paper. For a "clean" list of publications, please to [my Goole Scholar](https://scholar.google.com/citations?hl=en&user=ZK1dMoYAAAAJ&view_op=list_works) 

<h1>2023</h1>
<hr/>
**S. Zhang**, M. Chadwick, AGCP. Ramos, T. Parcollet, R. van Dalen, S. Bhattacharya. "[Real-Time Personalised Speech Enhancement Transformers with Dynamic
Cross-attended Speaker Representation](https://www.isca-speech.org/archive/pdfs/interspeech_2023/zhang23r_interspeech.pdf)" **INTERSPEECH**
<br/>**TL;DR**: We demonstrate that the cross-attention mechanism, despite its apparent computational expense, is more effective than conventional static single-vector approaches in learning speaker representations. Consequently, speech enhancement systems based on cross-attention outperform traditional models, achieving better performance with a smaller model size, which in turn results in faster speech inference.

T. Parcollet, **S. Zhang**, R. van Dalen, AGCP. Ramos, S. Bhattacharya. "[On the (In)Efficiency of Acoustic Feature Extractors for
Self-Supervised Speech Representation Learning](https://hal.science/hal-04116371/document)" **INTERSPEECH**
<br/>**TL;DR**: We carefully design the feature extractor frontend for self-supervised speech processing models, successfully reducing the minimum hardware requirements for training state-of-the-art (SOTA) models from A100 GPUs to RTX 3090 GPUs.

T. Parcollet^, R. van Dalen^, **S. Zhang^**, S Bhattacharya (^ equal contribution). "[Sumformer: A Linear-Complexity Alternative to
Self-Attention for Speech Recognition](https://arxiv.org/pdf/2307.07421.pdf)" (preprint. Paper to be updated soon.)
<br/>**TL;DR**: Our proposed linear alternative to self-attention reduces the VRAM usage by half and the training/inference time by up to 28%, while it outperforms the current state-of-the-art (SOTA) speech recognition models in English, French, Italian, Chinese, and Dutch datasets under three different acoustic conditions. The benefits can also be generalized to speech understanding.

T. Parcollet, H. Nguyen, S. Evain, M. Zanon Boito, A. Pupier, S. Mdhaffar, H. Le, S. Alisamir, N. Tomashenko, M. Dinarelli, **S. Zhang**, A. Allauzen, M. Coavoux, Y. Esteve, M. Rouvier, J. Goulian, B. Lecouteux, F. Portet, S. Rossato, F. Ringeval, D. Schwab, L. Besacier. "[LeBenchmark 2.0: a Standardized, Replicable and Enhanced Framework for
Self-supervised Representations of French Speech](https://arxiv.org/pdf/2309.05472.pdf)" (preprint)
<br/>**TL;DR**: We conducted benchmarks and open-sourced self-supervised learning models for French speech, which encompassed data ranging from 1,000 to 14,000 hours and model sizes from 26 million to 1 billion parameters. Additionally, we explored the pre-training and fine-tuning techniques for downstream tasks and their impact on the carbon footprint.


# 2022
<hr/>
M. Li, **S. Zhang**, C. Zorila, R. Doddipatla. “[Transformer-based Streaming ASR with Cumulative Attention.](https://arxiv.org/pdf/2203.05736.pdf)” **ICASSP**
<br/>**TL;DR**: We enhance the performance of Transformer-based encoder-decoder streaming speech recognition systems, achieving improvements in both speed and accuracy.

# 2021
<hr/>
**S. Zhang**, E. Loweimi, P. Bell, S. Renals. “[On the Usefulness of Self-Attention for Automatic Speech Recognition with Transformers.](https://arxiv.org/pdf/2011.04906.pdf)” **IEEE Spoken Language Technology Workshop (SLT)**
<br/>**TL;DR**: We unveil that for Transformer-based speech recognition systems, some self-attention layers can behave similarly to and can be replaced by linear layers. (Subsequent works show a similar conclusion has also been observed for state-of-the-art (SOTA) speech recognition systems based on [Conformer](https://openreview.net/pdf?id=AvcfxqRy4Y) and [Branchformer](https://arxiv.org/pdf/2207.02971.pdf).)

**S. Zhang**, C. Do, R. Doddipatla, E. Loweimi, P. Bell, S. Renals. “[Train Your Classifier First: Cascade Neural Networks Training from Upper Layers to Lower Layers.](https://arxiv.org/pdf/2102.04697.pdf)” **ICASSP**
<br/>**TL;DR**: We demonstrate that training neural networks layer by layer, starting from the upper layers (near the output) and progressing to the lower layers (near the input), can yield substantial and consistent performance gains for speech recognition, image classification, and language modeling tasks.

**S. Zhang**, E. Loweimi, P. Bell, S. Renals. “[Stochastic Attention Head Removal: A Simple and Effective Method for Improving Automatic Speech Recognition with Transformers.](https://arxiv.org/pdf/2011.04004v1.pdf)” **INTERSPEECH**
<br/>**TL;DR**: We show that not all attention heads are necessary in Transformer-based speech recognition systems. Removing attention heads randomly during training can improve the performance of state-of-the-art (SOTA) Transformer and Conformer speech recognition models. 
   
# 2020
<hr/>
**S. Zhang**, C. Do, R. Doddipatla, S. Renals. “[Learning Noise Invariant Features Through Transfer Learning for Robust End-to-End Speech Recognition.](https://www.pure.ed.ac.uk/ws/portalfiles/portal/138528386/Learning_Noise_Invariant_ZHANG_DOA24012020_AFV.pdf)” **ICASSP**
<br/>**TL;DR**: We show the upper layers (near the output) of the neural-based speech recognition models are more robust to noise and thus can be used to guide the lower layers of the network to learn noise-invariant features.

C. Do, **S. Zhang**, T. Hain. “[Selective Adaptation of End-to-End Speech Recognition using Hybrid CTC/Attention Architecture for Noise Robustness.](https://eurasip.org/Proceedings/Eusipco/Eusipco2020/pdfs/0000321.pdf)” **European Signal Processing Conference (EUSIPCO)**
<br/>**TL;DR**: “With a constraint on computational budget, we benchmark which part of LSTM-based speech recognition systems is the most effective for noise-robust adaptation using a very limited amount data (about 2.4 minutes).”

# 2019
<hr/>
**S. Zhang**, E. Loweimi, P. Bell, S. Renals. “[Windowed attention mechanisms for speech recognition.](https://www.pure.ed.ac.uk/ws/portalfiles/portal/80931064/WINDOWED_ATTENTION_MECHANISMS_FOR_SPEECH_RECOGNITION.pdf)” **ICASSP**
<br/>**TL;DR**: For the attentional encoder-decoder speech recognition system, we demonstrate restricting the attention mechanism to attend to a window of input frames with trained window length and shift will improve the accuracy and reduce the time complexity.  

**S. Zhang**, E. Loweimi, Y. Xu, P. Bell, S. Renals. “[Trainable Dynamic Subsampling for End-to-End Speech Recognition.](https://www.isca-speech.org/archive/pdfs/interspeech_2019/zhang19d_interspeech.pdf)” **INTERSPEECH**
<br/>**TL;DR**: We show a fully-trainable subsampling strategy for reducing the length of the speech input sequence gives better accuracies than then the conventional subsampling with a fixed sampling rate.

