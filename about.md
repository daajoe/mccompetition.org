---
layout: default
---

# The Problem: Model Counting

Given a Boolean formula the model counting problem, MC for short, asks to output the number of models (satisfying assignments) of a formula. If in addition each literal in the formula has an associated weight and we are interested in the sum of weights of all models, where the weight of a model is the product of the weights of its literals, we speak about weighted model counting (WMC).

---

## Applications

Many computational problems in modern society account to probabilistic reasoning, statistics, and combinatorics. Examples of such problems are identifying the reliability of energy infrastructure recognizing spam, or learning preference distributions, carrying out patient case simulations, or predicting weather. A variety of these real-world problems can be solved by representing the question in (Boolean) formulas and associating the number of models of the formula directly with the answer to the question.

---

## Computational Complexity

While the task of deciding whether a formula has a solution (SAT) is already known to be NP-complete, its generalization MC is even harder. Namely, MC is known to be #P-complete. Actually, this is computationally very hard, as for any problem in the polynomial hierarchy there is a deterministic polynomial-time Turing reduction to a the model counting problem or in other words every problem on the polynomial hierarchy can be solved polynomial-time by a machine that uses the model counting problem as an oracle.

---


