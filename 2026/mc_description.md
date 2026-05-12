---
---

# Model Counting Competition 2026

The competition will be co-located with the competitions at [SAT 2026](https://satisfiability.org/SAT26/).
<br><br>

[//]: # (<!--)
<b>[Pragmatics of SAT](https://www.pragmaticsofsat.org/2026/) invites Competition Solver Description Track.<br>
[The Workshop on Counting, Sampling, and Synthesis 2026](https://mccompetition.org/2026/mcw_description) also invites solver presentations.
</b>

[//]: # (-->)


## Tracks / Challenges
- Track 1: Model Counting
- ~~Track 2: Weighted Model Counting~~ (subsumed by Track 4)
- Track 3: Projected Model Counting
- Track 4: Projected Weighted Model Counting
- Track 5B: Algebraic Model Counting (AMC): Field (complex numbers)
<!--- - Track 6B: Bitvector Counting (tbd) --->

Track 2: Since the results no Track 2 were quite similar to Track 4 in 2024,
we omit weighted model counting unless requested by solver developer
who has not been participating in the competition.

Tracks 5 and 6 are bonus tracks, which will be experimental and
run in collaboration with the solver developers.

## Submission
See [submission instructions](submission) for details.
-  Please register in [this form (Benchmark Submissions)](https://forms.gle/XK1YMRRugMpt8wsz7)
-  Please register in [this form (Solver Submissions)](https://forms.gle/nQAwRxKu11UmLbVc8)

<!-- ## Results
The slides of the presentation of the results at SAT 2025 are available [here](../../assets/files/2025/mccomp_results_25.pdf).
--->

<!-- ## Instances
- [Instances for Track1--4](https://cloudstore.zih.tu-dresden.de/index.php/s/fiQ93PCPCX3EwDS) (last updated May 28, 2023) -->



## Rules
### Ranking
- A. Exact (arbitrary precision)
- ~~B. Exact (small precision loss)~~
- C. Approximate (provide approximation guarantee)
- D. Heuristic

### Restrictions
- Runtime: 3600s
- Memory: 32GB
- TempDisk Space: available for input transformation and preprocessing
- Precision (in relative error A,B,D):
  - Ranking A: 0.0 (any wrong solution results in removal from the ranking)
  - ~~Ranking B: 0.001 (more than 20 solutions outside margin results in disqualification)~~
  - Ranking C: $\alpha=0.8$ (more than 20 solutions outside margin results in removal from the ranking)
  - Ranking D: 20% (correct answer: 1 point, otherwise: 0 points)

### Benchmark Selection
We precompute instances and discard those that can be solved by
standard solvers within less than 10s and keep at most 40 instances
that cannot be solved by common existing solver.

## Public Instances
- tbd

<!-- 
- Tracks 1, 3, and 4: [link](https://nextcloud.liu.se/s/2zbn4APWnjLxRLo)
- Remaining tracks coming soon.
--> 

A few test instances are available in the [GitHub repository](https://github.com/arijitsh/mccomp-test-instances).

<!-- ## Public Results
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52720">Results on Public Instances for Track 1<a>
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52719">Results on Public Instances for Track 2<a>
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52718">Results on Public Instances for Track 3<a>
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52717">Results on Public Instances for Track 4<a> -->






## Format
We refer to a comprehensive
[document on the description of the competition format from 2021 (Updated June 2025 for new tracks)](../../assets/files/mccomp_format_25.pdf) for Tracks 1-5.

Note that **weights** may be given as **rational number** either as decimal number with at most
9 significant digits **or as fraction**.

For Track 5, we will decide about the format after discussing with interested developers (please send us an email).

<!-- For Track 6, we use the SMT format. -->

## Important Dates
Refer to the [submission and important dates page](dates).

## Organization

### Program Co-Chair / Organization
* Arijit Shaw (Chennai Mathematical Institute, India)
* Markus Hecher (CNRS, Artois University (CRIL), France)
* Johannes K. Fichte (Linköping University, Sweden)


### Judge
tbd
<!-- Mario Alviano --->

<!--
* Martin Gebser (AAU Klagenfurt, Austria)
-->
### Technical and Reproducibility Advisor
<!---
* Daniel Le Berre
--->

## Call for Benchmarks
Model Counting Competition invites extended submissions of collections of counting instances in the
an [DIMACS-like submission format](../../assets/files/mccomp_format_25.pdf).
See: [details](cfb2026.md)


- [Call for Benchmarks 2026 (PDF)](../../assets/files/2026/call_for_benchmarks2026.pdf)
- [Call for Benchmarks 2026](cfb2026)

### Evaluation Plattform
Pre-valuation will be run at the Swedish National Supercomputer Centre (NSC) and the
[Tetralith Cluster](https://www.nsc.liu.se/systems/tetralith/).

Submission will require a private github repository (or similar), from
where we can pull the solvers.


<!--- We are happy that the director of StarExec (Aaron Stump, Iowa)
accepted to host the model counting competition. The main part of the competition will
run on StarExec. We evaluate the solvers in parallel also on
the [Taurus Cluster in Dresden](https://www.top500.org/system/178555/).
--->





---
