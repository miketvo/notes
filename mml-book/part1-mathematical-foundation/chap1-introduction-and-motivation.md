# Chapter 1: Introduction and Motivation

**Abbreviations:**
- ML: Machine Learning

---


## The essentials of ML

1. Data $D$ (or dataset, experience $E$):
   $$D=\left\{(\textbf{x}_i,f(\textbf{x}_i))\right\}_{i=1}^n$$
   where:
    - $\textbf{x}$ is the features (attribute) vector.
    - $f(\textbf{x}_i)$ is the target feature.
    - $(\textbf{x}_i,f(\textbf{x}_i)$ for some $1<i<n$ is a data instance.
    - $n$ is the size of the data (number of data instances).

   $D$ can be thought of a table of $n$ rows, where $\textbf{x}_i$ are the attribute columns, $f(\textbf{x}_i)$ is the target column we will be predicting using our model, and each data instance $(\textbf{x}_i,f(\textbf{x}_i)$ is a row.

   All algorithms for ML make a significant assumption: The experience is a reasonable representation (or reasonable sample) of the true but unknown target function.
2. Model (or hypothesis): Function $h(\textbf{x})$
3. Learning:
    - Loss Function (Cost Function, Performance Measure $P$) measures how "wrong" the model is.
    - Optimization Procedure: To minimize $P$ to a reasonable level, but should never be 0, because it would be over-fitting and would not generalize well to new unseen data.

The end-goal of ML is to approximate the unknown target function $y=f(\textbf{x})$ (also called Task $T$) using the model $h(\textbf{x})$ by tuning its parameters to minimize the loss function $P$ to an "optimal" level (not over-fit nor under-fit). After this, $h(\textbf{x})$ can be used to predict the target feature of new unseen data.

In other words, the end-goal of ML is:
$$h(\textbf{x})\approx f(\textbf{x})\quad where\quad P_{optimal}$$

A model is said to learn from data if its performance on a given task $T$ improves with performance measure $P$ after the data $D$ (also called experience $E$) is taken into account.

The central challenge in machine learning is that our algorithm must perform well on new, previously unseen inputs (not just those on which our model was trained).

The ability to perform well on previously unseen inputs is called **generalization**.

- Generalization error is related to the true error of a hypothesis (cannot be measured).
- The generalization error of a machine learning model is typically estimated by measuring its performance on a test set collected separately from the training set.

Which is why after we have trained our model on our train dataset (data points to train the model) and validation dataset (to pick the best parameters and hyper-parameters for the model), we need to verify how well it generalize to new unseen data using a test dataset (not used for training).

But, the core challenge of ML is NOT ONLY:
- Collecting data
- Running algorithms
- Maximizing performance

The core challenge ML is ALSO in:
- Deciding what data to use.
- Deciding if an algorithm is suitable.
- Deciding the most suitable performance measure.
- Deciding which hypothesis is "the best" to use for a task.
- Making an ultimate judgement of how to approximate the unknown target function.
- Justify all of the above decisions with the stakeholders.


## Why study Mathematics for ML (theoretical study)?

- To create new ML solutions.
- Understand and debug existing solutions.
- Understand the limitations of ML.
- And more...
