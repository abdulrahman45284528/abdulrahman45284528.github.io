---
layout: default
title: Deep Learning
---
# Prerequisites
1. Advanced Applied Math
- Statistician Algebra (Linear Algebra + Statistics)
- Differentiation (Calculus: ODE + PDE)
- Probabilistic Number theory (Random Numbers)
- Abstract Algebra (theory)
2. Advanced Machine Learning
- Pattern Recognition
- Pattern Analysis
- Bias and Variance
- Optimization
- Regularization 

# Main steps in Deep Learning 
```
1. Problem Modeling:   Formulate a problem to model
2. Data curation:      To inform the model
3. Architecture Design:     To represent the model
    - Deep Feed Forward Networks (ANN) FFN
    - Convolutional Networks (CNN) --> ResNet, UNet
    - Sequence Modeling (RNNs)
    - Transformers (Attention mechanism)
    - Auto Encoder (AE)
    - Foundation Model
4. Loss Function:    Assess the performance of the model
5. Optimization:      To train the model
    - Regularization
    - Optimization
6. Evaluation Metrics:     For evaluation
    - IoU metric
    - Dice Metric
```

# Modern Practical Deep Learning
```
Type of Learning              | Description |

Supervised Learning           Learning with a teacher.
                              The model is provided with labelled examples and learns to map input data to corresponding output labels.
                              It's like learning from a textbook with answers provided. |
Unsupervised Learning         Learning without a teacher.
                              The model is given input data without explicit labels and must find patterns or structures in the data on its own.
                              It's like exploring a dataset without any prior knowledge or guidance. |
Semi-supervised Learning      Supervised Learning + Unsupervised Learning.
                              Learning with a limited teacher.
                              The model is trained on a combination of labelled and unlabeled data, leveraging both the provided labels and the inherent structure of the data to improve learning.
                              It's like having some answers but required to figure out the rest on your own. |
Self-supervised Learning      Form of Unsupervised Learning.
                              Learning from oneself.
                              The model generates its own labels from the input data and learns to predict some aspects of the data from other parts of the same data.
                              It's like creating puzzles for yourself and trying to solve them to understand the underlying patterns. |
Contrastive Learning          Type of Self-Supervised Learning
                              Learning through contrast.
                              The model learns representations by contrasting positive examples with negative examples, aiming to bring similar instances closer together and push dissimilar instances apart in the learned representation space.
                              It's like distinguishing between different examples to learn meaningful representations without explicit labels.
Reinforcement Learning        Learning through interaction.
                              The agent learns to make decisions by interacting with an environment and receiving feedback in the form of rewards or penalties.
                              It's like learning to play a game by trial and error. |
Active Learning               Learning with guidance.
                              The algorithm selects which data points to label, aiming to maximize learning efficiency by choosing the most informative instances for labelling.
                              It's like having a tutor who selects the most relevant exercises for you to practice. |
Transfer Learning	            Learning with prior knowledge.
                              The model leverages knowledge gained from solving one task and applies it to a related task, typically by fine-tuning or using it as a feature extractor.
                              It's like applying what you've learned in one subject to solve problems in another subject.
Meta-Learning	                Learning to learn.
                              The algorithm learns a learning strategy or optimization procedure that enables it to quickly adapt to new tasks or environments.
                              It's like developing study habits that help you learn new subjects more efficiently.
````



# Some Models
- Autoencoders
- Restricted Boltzmann Machines (RBMs)
- Generative Adversarial Networks (GANs)
- Variational Autoencoders (VAEs)
- Self-Organizing Maps (SOMs)
- Energy-Based Models (EBMs)
- Probabilistic Generative Models

# Some extra Learning types (Different training protocol)
- Unsupervised Representation Learning
- Multi-Modal and Multi-View Learning
- Continual Learning and Lifelong Learning
- Model-Based Reinforcement Learning
- Distributional Reinforcement Learning
- Hierarchical Reinforcement Learning

# Deep Reinforcement Learning
- Deep Q-Networks (DQN)
- Policy Gradient Methods
- Deep Deterministic Policy Gradient (DDPG)
- Twin Delayed DDPG (TD3)
- Soft Actor-Critic (SAC)
- Self-Play

#  Deep Learning Research
- Linear Factor Models
- Autoencoders
- Representation Learning
- Structured Probabilistic Models for Deep Learning
- Monte Carlo Methods
- Confronting the Partition Function
- Approximate Inference
- Deep Generative Models


