---
layout: post
title:  Machine Learning 공부
categories: MachineLearning
---
한글로 정리를 시작함.
대학원 졸업하고 거의 20년 만에 다시 공부를 시작하니,
20년간 세상은 많이 변했고... 나는 많이 늙고 많은 것들을 기억하지 못한다는 것을 새삼 느끼고 있음.

일단 아래의 3개의 카테고리에 대한 정리를 한 후에 각각에 대해서 개별적으로 다시 정리를 할 것임.

* Supervised Learning
* Unsupervised Learning
* Reinforcement Learning

wikipedia를 기반으로 영문 요약은 아래와 같음.
목표는 아래의 영어를.. 내가 소화할 수 있는 다른 쉬운 표현과 예제로 정리하는 것임.

#### Supervised Learning

<https://en.wikipedia.org/wiki/Supervised_learning>

Supervised learning is the machine learning task of inferring a function from labeled training data. The training data consist of a set of training examples. In supervised learning, each example is a pair consisting of an input object (typically a vector) and a desired output value (also called the supervisory signal). A supervised learning algorithm analyzes the training data and produces an inferred function, which can be used for mapping new examples. An optimal scenario will allow for the algorithm to correctly determine the class labels for unseen instances. This requires the learning algorithm to generalize from the training data to unseen situations in a "reasonable" way (see inductive bias).


#### Unsupervised Learning

<https://en.wikipedia.org/wiki/Unsupervised_learning>

Unsupervised machine learning is the machine learning task of inferring a function to describe hidden structure from "unlabeled" data (a classification or categorization is not included in the observations). Since the examples given to the learner are unlabeled, there is no evaluation of the accuracy of the structure that is output by the relevant algorithm—which is one way of distinguishing unsupervised learning from supervised learning and reinforcement learning.

A central case of unsupervised learning is the problem of density estimation in statistics,[1] though unsupervised learning encompasses many other problems (and solutions) involving summarizing and explaining key features of the data.


#### Reinforcement Learning

<https://en.wikipedia.org/wiki/Reinforcement_learning>

Reinforcement learning (RL) is an area of machine learning inspired by behaviourist psychology, concerned with how software agents ought to take actions in an environment so as to maximize some notion of cumulative reward. The problem, due to its generality, is studied in many other disciplines, such as game theory, control theory, operations research, information theory, simulation-based optimization, multi-agent systems, swarm intelligence, statistics and genetic algorithms. In the operations research and control literature, the field where reinforcement learning methods are studied is called approximate dynamic programming. The problem has been studied in the theory of optimal control, though most studies are concerned with the existence of optimal solutions and their characterization, and not with the learning or approximation aspects. In economics and game theory, reinforcement learning may be used to explain how equilibrium may arise under bounded rationality.

In machine learning, the environment is typically formulated as a Markov decision process (MDP), as many reinforcement learning algorithms for this context utilize dynamic programming techniques.[1] The main difference between the classical techniques and reinforcement learning algorithms is that the latter do not need knowledge about the MDP and they target large MDPs where exact methods become infeasible.

Reinforcement learning differs from standard supervised learning in that correct input/output pairs are never presented, nor sub-optimal actions explicitly corrected. Instead the focus is on on-line performance, which involves finding a balance between exploration (of uncharted territory) and exploitation (of current knowledge).[2] The exploration vs. exploitation trade-off in reinforcement learning has been most thoroughly studied through the multi-armed bandit problem and in finite MDPs.
