---
title: Miscellaneous
layout: home
excerpt: A collection of mini-projects and short writeups
order: 8
---

A collection of short-writeups and projects from the past few years.

**Table of Contents**
- [Internal Coherence Maximisation (CIM) Implementation](#internal-coherence-maximisation-cim-implementation)
- [Can synthetic data unblock the training data bottleneck?](#can-synthetic-data-unblock-the-training-data-bottleneck)
- [Representation Learning](#representation-learning)


## Internal Coherence Maximisation (CIM) Implementation
A core problem in training smarter-than-human AI systems is providing a reliable feedback signal to the AI's outputs. Human labelling of outputs suffers from being too expensive, and potentially inaccurate for tasks that exceed human ability. [Wen et al. (2025)](https://arxiv.org/abs/2506.10139) develop the ICM algorithm to generate labels without human supervision, by choosing the label set that maximises a combination of (a). internal coherence **between the generated label set**, and (b) logical consistency. I implemented this [here](https://github.com/IyngkarranKumar/ICM_implementation/tree/main).

## Can synthetic data unblock the training data bottleneck?
Large language models read through the entire internet during the process of pretraining, equipping them with a vast store of knowledge. However, there's only one internet, which leaves the question of how pretraining datasets will continue grow to accomodate larger models once internet data has been exhausted. One option is to generate synthetic data from existing LLMs and train on that, but it is an open question as to how effective this is. In early 2024, I wrote a blog post to get a better sense of the key factors that influence the substitutability of human-generated data with model-generated data. See [here](/assets/docs/synthetic_data_blog.pdf) for the full post.  

## Representation Learning
To what extent do frontier AI systems learn representations of training data that are similar to human representations? Are some abstractions more [''natural''](https://www.lesswrong.com/w/natural-abstraction) than others; that is, will most intelligent systems converge to the same representation of a concept? These are important, lofty questions, the answers to which will have significant implications to the science of deep learning and AI alignment. With this in mind, I spent some time in summer 2022 developing a better understanding of representation learning, as well as background concepts in information theory. A write-up is [here](/assets/docs/Learning_Representations.pdf). 