---
layout: post
title:  Supervised Learning
categories: Machine Learning
---

* Linear Regression
* Logistic Regression
* Softmax Regression (Multinomial Logistic Regression)
* Back Propagation

#### Linear Regression

<https://en.wikipedia.org/wiki/Linear_regression>

In statistics, linear regression is a linear approach for modeling the relationship between a scalar dependent variable y and one or more explanatory variables (or independent variables) denoted X. The case of one explanatory variable is called simple linear regression. For more than one explanatory variable, the process is called multiple linear regression.[1] (This term is distinct from multivariate linear regression, where multiple correlated dependent variables are predicted, rather than a single scalar variable.)[2]

#### Logistic Regression

<https://en.wikipedia.org/wiki/Logistic_regression>

In statistics, logistic regression, or logit regression, or logit model[1] is a regression model where the dependent variable (DV) is categorical. This article covers the case of a binary dependent variable—that is, where the output can take only two values, "0" and "1", which represent outcomes such as pass/fail, win/lose, alive/dead or healthy/sick. Cases where the dependent variable has more than two outcome categories may be analysed in multinomial logistic regression, or, if the multiple categories are ordered, in ordinal logistic regression.[2] In the terminology of economics, logistic regression is an example of a qualitative response/discrete choice model.

Logistic regression was developed by statistician David Cox in 1958.[2][3] The binary logistic model is used to estimate the probability of a binary response based on one or more predictor (or independent) variables (features). It allows one to say that the presence of a risk factor increases the odds of a given outcome by a specific factor.

#### Softmax Regression (Multinomial Logistic Regression)

<https://en.wikipedia.org/wiki/Multinomial_logistic_regression>

In statistics, multinomial logistic regression is a classification method that generalizes logistic regression to multiclass problems, i.e. with more than two possible discrete outcomes.[1] That is, it is a model that is used to predict the probabilities of the different possible outcomes of a categorically distributed dependent variable, given a set of independent variables (which may be real-valued, binary-valued, categorical-valued, etc.).

Multinomial logistic regression is known by a variety of other names, including polytomous LR,[2][3] multiclass LR, softmax regression, multinomial logit, maximum entropy (MaxEnt) classifier, conditional maximum entropy model.[4]


#### Back Propagation

<https://en.wikipedia.org/wiki/Backpropagation>

Backpropagation is a method used in artificial neural networks to calculate the error contribution of each neuron after a batch of data (in image recognition, multiple images) is processed. It is a special case of an older and more general technique called automatic differentiation. In the context of learning, backpropagation is commonly used by the gradient descent optimization algorithm to adjust the weight of neurons by calculating the gradient of the loss function. This technique is also sometimes called backward propagation of errors, because the error is calculated at the output and distributed back through the network layers.

The backpropagation algorithm has been repeatedly rediscovered and is equivalent to automatic differentiation in reverse accumulation mode. Backpropagation requires a known, desired output for each input value—it is therefore considered to be a supervised learning method (although it is used in some unsupervised networks such as autoencoders). Backpropagation is also a generalization of the delta rule to multi-layered feedforward networks, made possible by using the chain rule to iteratively compute gradients for each layer. It is closely related to the Gauss–Newton algorithm, and is part of continuing research in neural backpropagation. Backpropagation can be used with any gradient-based optimizer, such as L-BFGS or truncated Newton[citation needed][clarification needed].

Backpropagation is commonly used to train deep neural networks [1], a term used to describe neural networks with more than one hidden layer.[2]

#### Recurrent Neural Network (RNN)

<http://karpathy.github.io/2015/05/21/rnn-effectiveness/>

기본적으로 history 에 대한 정보를 가지는 문제를 푸려고 하는 것임.\\
예를 들어서 언어의 인식, 번역등을 context에 대한 정보가 필요함.\\
자동 자막생성도 비슷한 것으로...\\
어떤 단어의 뉘앙스를 파악하기 위해서는 해당 단어가 어떤 context로 사용되었는지에 대한 이해가 필요함.\\
이에, 네트웍의 구조를 보면 n-1번째 iteration 의 ouput이 n번째 iteration의 input 으로도 들어감.

여기에 그림하나 넣어두자....

#### Long Short Term Memory(LSTM)

<http://colah.github.io/posts/2015-08-Understanding-LSTMs/>

위의 블로그에 잘 설명을 해두었는데...\\
기본적으로 RNN의 구조에서 어떤 경우에는 n-1번째 iteration의 output보다 n-t번째 iteration의 output이 더 중요할 때도 있음.\\
예를 들어서 번역의 경우, 바로 전의 단어보다 앞 문장의 특정 단어가 더 중요한 경우가 존재함.\\
이런 경우를 어떻게 모델링할 것이냐에 대한 것임.

자세한 분석, 설명을 추후에 추가하기로 함.
