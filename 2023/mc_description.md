---
---

# Model Counting Competition 2023

The competition will be co-located with the competitions at SAT 2023. 
<br><br>

<center><b>Send us an email and stay tuned.</b></center>

## Tracks / Challenges
1. **Model Counting (mc)**<br/>
2. **Weighted Model Counting (wmc)**<br/>
3. **Projected Model Counting (pmc)**<br/>
4. **Projected Weighted Model Counting (pwmc)**<br/>

## Call for Benchmarks
Model Counting Competition invites extended submissions of collections of counting instances in the 
an [DIMACS-like submission format as used in the 2021 competition](../../assets/files/2021/competition2021.pdf).

<!-- - [Call for Benchmarks 2023 (PDF)](../../assets/files/2022/call_for_benchmarks2022.pdf) -->
- [Call for Benchmarks 2023 (TEXT)](cfb2023)

## Rules
### Ranking
- A. Exact (arbitrary precision)
- B. Exact (small precision loss)
- C. Approximate (provide approximation guarantee)
- D. Heuristic (experimental)

### Restictions
- Runtime: 3600s
- Memory: 32GB
- TempDisk Space: available for input transformation and preprocessing
- Precision (in relative error A,B,D): 
  - Ranking A: 0.0 (any wrong solution results in disqualification)
  - Ranking B: 0.001 (more than 20 solutions outside margin results in disqualification)
  - Ranking C: $\alpha=0.8$ (more than 20 solutions outside margin results in disqualification)
  - Ranking D: 20% (correct answer: 1 point, otherwise: 0 points)

### Benchmark Selection
We precompute instances and discard those that can be solved by
standard solvers within less than 10s and keep at most 40 instances
that cannot be solved by common existing solver. 

## Instances
- [Instances for Track1--4](https://cloudstore.zih.tu-dresden.de/index.php/s/fiQ93PCPCX3EwDS) (last updated May 28, 2023)

- 

## Important Dates
see [Dates](dates)

## Public Results
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52720">Results on Public Instances for Track 1<a>
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52719">Results on Public Instances for Track 2<a>
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52718">Results on Public Instances for Track 3<a>
- <a href="https://www.starexec.org/starexec/secure/details/job.jsp?id=52717">Results on Public Instances for Track 4<a>


  
## Submission
Register an Account with [StarExec](https://www.starexec.org/starexec/secure/explore/spaces.jsp?id=441292).
 We will give you access and you will be able to upload your solver there.


## Format
We refer to a comprehensive 
[document on the description of the competition format from 2021](../../assets/files/2021/competition2021.pdf). 

## Important Dates (preliminary)
- December 15, 2021: Call for Benchmarks
- December 20, 2021: 1st Call for Participation
- February 15, 2022: Deadline for Benchmark Submission (submit asap)<br>
  Please use the [Google Form](https://tinyurl.com/32m78k32)
- ~~April 27, 2022~~ May 14, 2022: Testing Benchmarks / Public Instances Released</b>
- ~~April 30, 2022~~ May 22, 2022: Intent to Participate: Please use the [Google Form](https://tinyurl.com/2p9db6sa)
- ~~May 12, 2022~~ May 22, 2022: Submission Deadline
- <b>June 30, 2022: Participants are notified about their public results</b>
- Jul 7, 2022 (estimated): Participants are notified about their private results 
- Jul 14, 2022: Comments Deadline by Participants
- Aug 4, 2022: FLoC Presentation of the Results
- Aug 11, 2022: Workshop on Counting and Sampling (PostFLoC Workshop)

- March 15, 2022: Benchmarks Evalutated
- March 31, 2022: Competition Benchmarks Chosen
 - April 1, 2022: Submission System (StarExec) available 
--->

## Organization

### Program Co-Chair
* Markus Hecher (MIT, MA, United States)
* Johannes K. Fichte (Linköping University, Sweden)

### Judge
* Martin Gebser (AAU Klagenfurt, Austria) 

### Technical and Reproducibility Advisor
* Daniel Le Berre 

### Evaluation Plattform 
We are happy that the director of StarExec (Aaron Stump, Iowa) 
accepted to host the model counting competition. The main part of the competition will 
run on StarExec. We evaluate the solvers in parallel also on 
the [Taurus Cluster in Dresden](https://www.top500.org/system/178555/). 

<!---
## Sponsors
[data-experts](https://data-experts.de) already announced sponsoring of MC 2022.
--->


---
