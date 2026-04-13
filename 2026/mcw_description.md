---
---

# Workshop on Counting, Sampling, and Synthesis 2026

<!--- 
## Registration

[Registration for CP, SAT, SoCS, and affiliated workshops is now open!](https://cp2025.a4cp.org/registration.html)
--->

## Purpose

The _Workshop on Counting, Sampling, and Synthesis_ is an event for researchers in model counting and sampling. It
covers advanced topics such as weighted and projected counters/samplers and various domains such as SAT, SMT, ASP, and
CP. The workshop has expanded its focus to include the role of model counters, samplers, and solvers in the area of
automated synthesis. The goal of the workshop is to facilitate the exchange of cutting-edge theoretical and practical
insights, with a particular emphasis on innovative solver technologies and their real-world applications. Additionally,
the workshop provides an opportunity for developers of model counters to showcase their work and share detailed
competition results, to encourage discussions that bridge theory and practice.

## Venue

This year’s event will be held alongside other workshops at FLoC 2026 (affiliated with the SAT 2026) conference.
For more information, please visit the [FLoC 2026 website](https://www.floc26.org/program).

## Date

Day: Saturday, July 25th, 2026

## Schedule

<style>
td, th {
    border: 1px solid grey
}
table th:first-of-type {
    width: 10%;
}
table th:nth-of-type(2) {
    width: 55%;
}
table th:nth-of-type(3) {
    width: 35%;
}

</style>

<!--
| Time | Title | Author(s)/ Presenter |
|-------|:---------|-------|
| 10.30-11.00 | ☕ Coffee Break ||
| 11.00-11.10 | Introductory Remarks ||
| 11.10-11.40 | Approximate SMT Counting Beyond Discrete Domains<details>Satisfiability Modulo Theory (SMT) solvers have advanced automated reasoning, solving complex formulas across discrete and continuous domains. Recent progress in propositional model counting motivates extending SMT capabilities toward model counting, especially for hybrid SMT formulas. Existing approaches, like bit-blasting, are limited to discrete variables, highlighting the challenge of counting solutions projected onto the discrete domain in hybrid formulas.<br><br>We introduce pact, an SMT model counter for hybrid formulas that uses hashing-based approximate model counting to estimate solutions with theoretical guarantees. pact makes a logarithmic number of SMT solver calls relative to the projection variables, leveraging optimized hash functions. pact achieves significant performance improvements over baselines on a large suite of benchmarks. In particular, out of 14,202 instances, pact successfully finished on 603 instances, while Baseline could only finish on 13 instances.</details> | <b>Arijit Shaw</b> and Kuldeep S. Meel |
| 11.40-12.10 | Numerical Considerations in Weighted Model Counting<details>Weighted model counting computes the sum of the rational-valued weights associated with the satisfying assignments for a Boolean formula, where the weight of an assignment is given by the product of the weights assigned to the positive and negated variables comprising the assignment. Weighted model counting finds applications across a variety of domains including probabilistic reasoning and quantitative risk assessment.<br><br>Most weighted model counting programs operate by (explicitly or implicitly) converting the input formula into a form that enables arithmetic evaluation, using multiplication for conjunctions and addition for disjunctions. Performing this evaluation using floating-point arithmetic can yield inaccurate results, and it cannot quantify the level of precision achieved. Computing with rational arithmetic gives exact results, but it is costly in both time and space.<br><br>This paper describes how to combine multiple numeric representations to efficiently compute weighted model counts that are guaranteed to achieve a user-specified precision. When all weights are nonnegative, we prove that the precision loss of arithmetic evaluation using floating-point arithmetic can be tightly bounded. For problems with negative weights, we show that a combination of interval floating-point arithmetic and rational arithmetic can achieve the twin goals of efficiency and guaranteed precision. For our evaluations, we have devised especially challenging formulas and weight assignments, in order to maximize the robustness of our result.</details>| <b>Randal Bryant</b> |
| 12.30-13.30 | 🍽️ Lunch ||
| 13.30-14.00 | Cara: An Isomorphism-Based #SAT Solver<details>We introduce Cara, a novel #SAT solver that leverages the Cara caching scheme. This scheme uses approximate isomorphism detection through literal renaming to identify equivalent residual CNF formulae, thereby improving cache efficiency. In addition, Cara incorporates adaptive dynamic decomposition, selecting hypergraph partitioning modes/tools according to runtime cache statistics to balance cut quality and computational cost. Combined, these techniques reduce redundant computation and enhance the overall efficiency of model counting.</details> | <b>Petr Illner</b> |
| 14.00-14.30 | Surveying the Model Counting Competition 2025| <b>Johannes K. Fichte</b>, Markus Hecher and Arijit Shaw |
| 14.30-15.00 | Towards Real-Time Approximate Counting<details>Model counting is the task of counting the number of satisfying assignments of a Boolean formula. Since counting is intractable in general, most applications use (ε, δ)-approximations, where the output is within a (1 + ε)-factor of the count with probability at least 1 − δ. Many demanding applications make thousands of counting queries, and the state-of-the-art approximate counter, ApproxMC, makes hundreds of calls to SAT solvers to answer a single approximate counting query. The sheer number of SAT calls poses a significant challenge to the existing approaches.<br><br>In this work, we propose an approximation scheme, ApproxMC7 that is tailored to such demanding applications with low time limits. Compared to ApproxMC, ApproxMC7 makes 14× fewer SAT calls while providing the same guarantees as ApproxMC in the constant-factor regime. In an evaluation over 2,247 instances, ApproxMC7 solved 271 more instances and achieved a 2× speedup against ApproxMC.</details> | Yash Pote, Kuldeep S. Meel and <b>Jiong Yang</b> |
|15.00-15.30| ☕ Coffee Break & End of Workshop ||
-->

## Timeline

See [Dates](dates).

## Format

You can showcase your best work in counting, sampling, or synthesis, whether it has been published elsewhere or not.
Presenters can choose between giving a talk or presenting a poster. Each talk will have a 20-minute time slot for the
presentation, followed by a 10-minute Q&A session.

## Submissions

There are no specific format requirements for the submission. We expect you to provide a reasonable description in PDF
format.

- **Submission.**  Please upload a PDF on [FLoC HotCRP MC](https://submissions.floc26.org/mc/).
- **Procedure for selecting papers.** All submissions will be reviewed by 1-2 program committee members, who will make
  recommendations for paper selection.
- **Plans for dissemination.** There will be no proceedings, but the abstracts and slides will be made available on the
  website.

## Contact

If you have any questions about the workshop, the best way to contact the organizers is by
emailing <span style="color:blue">mcw at modelcounting.org</span>.

## Team

### Organizers

- [Johannes K. Fichte](https://liu.se/en/employee/johfi52) (Linköping University, Sweden)
- [Markus Hecher](https://dbai.tuwien.ac.at/staff/hecher/) (French National Centre for Scientific Research (CNRS),
  University d'Artois (CRIL), France)
- [Kuldeep S. Meel](http://www.kuldeepmeel.com/) (Georgia Institute of Technology, USA)

---
