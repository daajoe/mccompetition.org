---
layout: default
---

# The Problems: 

## Model Counting (mc)

- Given: a Boolean formula F;
- Task: output the number of models (satisfying assignments) of the formula F. 

## Weighted Model Counting (wmc) 
- Given: a Boolean formula F and a weight for each literal that occurs in F; 
- Task: output sum of weights of all models, where the weight of a model is the product of the weights of its literals.


## Projected Model Counting (pmc) 
- Given: a Boolean formula F and a set P of projection variables; 
- Task: output the number of models of F that are different when models are restricted to the variables that occur in P.



---

## Applications

Many computational problems in modern society account to probabilistic reasoning, statistics, and combinatorics. Examples of such problems are identifying the reliability of energy infrastructure recognizing spam, or learning preference distributions, carrying out patient case simulations, or predicting weather. A variety of these real-world problems can be solved by representing the question in (Boolean) formulas and associating the number of models of the formula directly with the answer to the question.

---

## Computational Complexity

While the task of deciding whether a formula has a solution (SAT) is already known to be NP-complete, its generalization (W)MC is even harder. Namely, (W)MC is known to be #P-complete. Actually, this is computationally very hard, as for any problem in the polynomial hierarchy there is a deterministic polynomial-time Turing reduction to a the model counting problem or in other words every problem on the polynomial hierarchy can be solved polynomial-time by a machine that uses the model counting problem as an oracle.

---


