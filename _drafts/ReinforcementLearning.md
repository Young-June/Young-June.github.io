---
layout: post
title:  Reinforcement Learning
categories: Machine Learning
---


* Q Learning



#### Q Learning

<https://en.wikipedia.org/wiki/Q-learning>

Q-learning is a model-free reinforcement learning technique. Specifically, Q-learning can be used to find an optimal action-selection policy for any given (finite) Markov decision process (MDP). It works by learning an action-value function that ultimately gives the expected utility of taking a given action in a given state and following the optimal policy thereafter. A policy is a rule that the agent follows in selecting actions, given the state it is in. When such an action-value function is learned, the optimal policy can be constructed by simply selecting the action with the highest value in each state. One of the strengths of Q-learning is that it is able to compare the expected utility of the available actions without requiring a model of the environment. Additionally, Q-learning can handle problems with stochastic transitions and rewards, without requiring any adaptations. It has been proven that for any finite MDP, Q-learning eventually finds an optimal policy, in the sense that the expected value of the total reward return over all successive steps, starting from the current state, is the maximum achievable.[1]


#### Markov decision process (MDP)

<https://en.wikipedia.org/wiki/Markov_decision_process>

Markov decision processes (MDPs) provide a mathematical framework for modeling decision making in situations where outcomes are partly random and partly under the control of a decision maker. MDPs are useful for studying a wide range of optimization problems solved via dynamic programming and reinforcement learning. MDPs were known at least as early as the 1950s (cf. Bellman 1957); a core body of research on Markov decision processes resulted from Ronald A. Howard's book published in 1960, Dynamic Programming and Markov Processes.[1] They are used in a wide area of disciplines, including robotics, automatic control, economics, and manufacturing.

More precisely, a Markov decision process is a discrete time stochastic control process. At each time step, the process is in some state {\displaystyle s} s, and the decision maker may choose any action {\displaystyle a} a that is available in state {\displaystyle s} s. The process responds at the next time step by randomly moving into a new state {\displaystyle s'} s', and giving the decision maker a corresponding reward {\displaystyle R_{a}(s,s')} R_a(s,s').

The probability that the process moves into its new state {\displaystyle s'} s' is influenced by the chosen action. Specifically, it is given by the state transition function {\displaystyle P_{a}(s,s')} P_a(s,s'). Thus, the next state {\displaystyle s'} s' depends on the current state {\displaystyle s} s and the decision maker's action {\displaystyle a} a. But given {\displaystyle s} s and {\displaystyle a} a, it is conditionally independent of all previous states and actions; in other words, the state transitions of an MDP satisfies the Markov property.

Markov decision processes are an extension of Markov chains; the difference is the addition of actions (allowing choice) and rewards (giving motivation). Conversely, if only one action exists for each state (e.g. "wait") and all rewards are the same (e.g. "zero"), a Markov decision process reduces to a Markov chain.
