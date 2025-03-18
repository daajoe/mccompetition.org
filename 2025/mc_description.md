---
---

# Model Counting Competition 2025

The competition will be co-located with the competitions at [SAT 2025](http://satisfiability.org/SAT25/)
(expected).
<br><br>

[//]: # (<!--)
<b>[Pragmatics of SAT](http://www.pragmaticsofsat.org/2025/) invites Competition Solver Description Track.<br>
[The Workshop on Counting, Sampling, and Synthesis 2025](https://mccompetition.org/2025/mcw_description) also invites solver presentations.
</b>

[//]: # (-->)


## Tracks / Challenges
- Track 1: Model Counting
- ~~Track 2: Weighted Model Counting~~ (subsumed by Track 4)
- Track 3: Projected Model Counting
- Track 4: Projected Weighted Model Counting
- Track 5B: Algebraic Model Counting (AMC): Field (tbd) 
- Track 6B: Bitvector Counting

Since Track 2 is subsumed by Track 4 and results were quite similar in 2024, 
we omit weighted model counting unless requested by solver developer 
who has not been participating in the competition.

Tracks 5 and 6 are bonus tracks, which will be experimental and
run in collaboration with the solver developers.

## Results

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

<!-- ## Public Results
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52720">Results on Public Instances for Track 1<a>
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52719">Results on Public Instances for Track 2<a>
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52718">Results on Public Instances for Track 3<a>
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52717">Results on Public Instances for Track 4<a> -->



## Submission
Please register in [this form](https://tinyurl.com/ycx3w4cd).

TBD


## Format
We refer to a comprehensive
[document on the description of the competition format from 2021 (Updated June 2024)](../../assets/files/mccomp_format_24.pdf) for Tracks 1-4.
Note that **weights** may be given as **rational number** either as decimal number with at most 
9 significant digits **or as fraction**.

For Track 5, we will decide about the format after discussing with interested developers (please send us an email).

For Track 6, we use the SMT format.

## Important Dates (Tentative)
Refer to the [submission and important dates page](dates).

## Organization

### Program Co-Chair / Organization
* Arijit Shaw (Chennai Mathematical Institute, India)
* Markus Hecher (MIT, MA, United States)
* Johannes K. Fichte (Linköping University, Sweden)


### Judge
tba

<!--
* Martin Gebser (AAU Klagenfurt, Austria)
-->
### Technical and Reproducibility Advisor
tba

<!---
* Daniel Le Berre
--->

## Call for Benchmarks
Model Counting Competition invites extended submissions of collections of counting instances in the
an [DIMACS-like submission format (updated June'24)](../../assets/files/mccomp_format_24.pdf).
See: [details](cfb2025.md)


- [Call for Benchmarks 2025 (PDF)](../../assets/files/2025/call_for_benchmarks2025.pdf)
- [Call for Benchmarks 2025](cfb2025)

### Evaluation Plattform
We are happy that the Software and Computational Systems (SoSy) Lab at 
Ludwig Maximilian University of Munich accepted to host the model counting competition.
Thank you Dirk Beyer and Philipp Wendler.

Pre-valuation will be run at the Swedish National Supercomputer Centre (NSC) and the Tetralith Cluster.  
(Note that StarExec Iowa is about to be decommissioned in 2025).


<!--- We are happy that the director of StarExec (Aaron Stump, Iowa)
accepted to host the model counting competition. The main part of the competition will
run on StarExec. We evaluate the solvers in parallel also on
the [Taurus Cluster in Dresden](https://www.top500.org/system/178555/).
---> 





---
