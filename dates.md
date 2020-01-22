---
---

# Important Dates

- December 18th, 2019: Announcement of the challenge (Tracks)
- January 22nd, 2019: Call for Benchmarks
- May 22th, 2020 (AoE)  -- Deadline (DS) -- Submission
- June 3rd, 2020 (AoE) -- Deadline (DD) -- Submission of a solver description via Easychair



<!-- November 16th, 2018: Announcement of the tracks and additional informations (input formats and problem feasibility checker are available online)
December 10th, 2018: Public htd instances are available
January 7th, 2019: Public vc instances are available
March 8th, 2019: Leaderboard online (by organizers) and submission *open* for preliminary versions (bugfixing for the authors and initial comparison on public instances)-->

<!-- July 1st, 2019: Announcement of the results
September 11-13, 2019 (International Symposium on Parameterized and Exact Computation ([IPEC 2019](http://fpt.wikidot.com/ipec)) in Munich, Germany)
 Award ceremony
 Poster Session (tbd) -->



---

# Submission Information

## Call for Benchmarks

Model Counting Competition MC 2020 invites submission of collections of (weighted) model counting instances in the standard DIMACS-based submission formats as given at 
the [competition tracks](model-counting-competition).

### Submission Procedure

A benchmark submission should consist of a single zip or gzipped tar package, containing the instance files and a description of the benchmarks.
Please use appropriate file naming conventions, where suited. Ideally, each instance file name should contain a short descriptive part for the problem domain as well as the parameters used for generating the instance as applicable.
The benchmark description description must be be submitted as PDF. The description should include author information with affiliations, a description of the problem domains, a description of the parameters used for generating the instances, and the file name convention. References should be used as appropriate.
The benchmark descriptions will be posted on the MC 2020 website. Furthermore, the organizers are considering publishing the collection of system and benchmark descriptions on arxiv.
Please submit benchmarks by email to [benchmarks@mccompetition.org](mailto:benchmarks@mccompetition.org) using the subject title "MC 2020 benchmark submission" by *March 5 AoE* the latest.

## Call for Participation

#### Registration
1. Register at optil.io (<https://www.optil.io/optilion/login>)
2. Access Easychair (<https://easychair.org/conferences/?conf=mc2020>) and register your group 
   - Use as title of the paper your login name at optil
   - Place the name of your solver in the abstract
3. Submit your solution via optil (as soon as the optil submission is open) 


#### Requirements
1. As programming languages we plan to allow C, C++, C#, Java8, Java10, Python2, Python3, Rust, and VB.NET. 
2. Open Source (e.g. GPL, MIT, or public domain)
3. Source code is available on a public repository (e.g., [Bitbucket](https://bitbucket.org), [GitHub](https://github.com), [Gitlab](https://gitlab.com)).
**Note:** We allow a limited use of external dependencies. These external dependencies may include commercial solvers such as [IBM Cplex](http://www-01.ibm.com/software/integration/optimization/cplex-optimizer), [gurobi](https://www.gurobi.com/), as well as open source solvers. 
 However, please contact us in advance, since we need to get it running on optil.io. 
4. Submissions Solver: Deadline (DS)
   1. Submission via [optil.io](https://www.optil.io/optilion/)
   2. Register solver and participants via [EasyChair](https://easychair.org/conferences/?conf=mc2020)
   3. Create a release in the public repository of the solver (name: mc-2020)
5. Submission Description: Deadline (DD)
   1. Place the source code of the solver in a digital library (e.g., [Zenodo](https://zenodo.org/)) and generate a DOI 
   2. Submit solver description via [EasyChair](https://easychair.org/conferences/?conf=mc2020) use DOI to refer to the solver and include a reference to the public source code repository 
<!--For parallel solving on GPUs, we aim for Nvidia cuda.-->



#### Solver

- Content of the Repository 
  -  LICENSE.md or LICENSE.txt file at the root
  -  README.md or README.txt file at the root
  -  INSTALL.md or INSTALL.txt file at the root that contains the requirements for external libraries 
      -  Language specific file for easy installation (e.g., *CMakeLists.txt* for cmake or *environment.yaml* for anaconda); the file is not mandatory, however, we encourage to provide it at the time of the submission of the solver description


#### Solver Description
- 2+ pages
- Should briefly describe the used techniques and references to the original publications. 

---
