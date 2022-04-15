---
layout: single
title: "Toward Human Cognition-inspired High-Level Decision Making For Hierarchical Reinforcement Learning Agents"
excerpt: "Hierarchical reinforcement learning (HRL) methods aim to leverage the concept of temporal abstraction to efficiently solve long-horizon, sequential decision-making problems with sparse and delayed rewards. However, the decision-making process of the agent in most HRL methods is often based directly on low-level observations, while also using fixed temporal abstraction. We propose the hierarchical world model (HWM), which can capture more flexible high-level, temporally abstract dynamics, as well as low-level dynamics of the system.
We posit such model is a natural extension to the HRL framework toward a decision-making process closer to that of humans."

tags:
  - Reinforcement Learning
  - Hierarchical Reinforcement Learning
  - Hierarchical World Model
  - World Models
  - Implementation
  - Research
  - Graphical Model
  - Publication
  - Paper
comments: true
classes: wide
---

### Rousslan Fernand Julien Dossa, Takashi Matsubara

In this paper, we propose a hierarchically structured world model that would separate the internal state of the system (task) into two-level hierarchy of latent variables.
The low-level latent variables is expected to encode fast-changing elements of a given RL task, while the high-level of the hierarchy would encode slowly changing elements.
The latter are approximated using variational temporal abstraction.

<embed src="/assets/publications/pdfs/2021_ieice_ccs_toward_human_cognition_inspired_high_level_decision_making_for_hrl.pdf" type="application/pdf" />

Preliminary results were also presented at [2021 Non Linear Science Workshop](https://nlsw2021.org/) with the following extended summary:

<embed src="/assets/publications/pdfs/2021_NOLTA_Non_Linear_Science_Workshop_Hierarchical_World_Model_Extend_Summary_Compressed.pdf" type="application/pdf" />
