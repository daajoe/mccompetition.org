---
---
# Model Counting Competition: Submission Information

## Tracks / Challenges
1. *Model Counting (mc)*
(Compute the number of satisfying assignments to a given CNF):<br/>
[Details for the track (Formats)](mc_format#track-1-model-counting)<br/>
[Optil Test Submission (Lite Track / allows to test your parser etc...)](https://www.optil.io/optilion/problem/3183)<br/>
[**Optil Track Submission**](https://www.optil.io/optilion/problem/3186)<br/>

2. *Weighted Model Counting (wmc)*
(Compute the weighted model count of a given CNF and weights):<br/>
[Details for the track (Formats)](mc_format#track-2-weighted-model-counting)<br/>
[Optil Test Submission (Lite Track / allows to test your parser etc...)](https://www.optil.io/optilion/problem/3184)<br/>
[**Optil Track Submission**](https://www.optil.io/optilion/problem/3187)<br/>


3. *Projected Model Counting (pmc)*
(Compute the projected model count of a given CNF and projection variables):<br/>
[Details for the track (Formats)](mc_format#track-3-projected-model-counting)<br/>
[**Optil Test Submission** (Lite Track / allows to test your parser etc...)](https://www.optil.io/optilion/problem/3185)<br/>
[Optil Track Submission (TBA)](https://www.optil.io/optilion/problem/3188)<br/>

## Call for Benchmarks

Model Counting Competition MC 2020 invites submission of collections of (weighted) model counting instances in the 
standard DIMACS-based submission formats as given at the [competition tracks and format](mc_format).

### Submission Procedure

A benchmark submission should consist of a single zip or gzipped tar package, containing the instance files and a description of the benchmarks.
Please use appropriate file naming conventions, where suited. Ideally, each instance file name should contain a short descriptive part for the problem domain as well as the parameters used for generating the instance as applicable.
The benchmark description must be submitted as PDF. The description should include author information with affiliations, a description of the problem domains, a description of the parameters used for generating the instances, and the file name convention. References should be used as appropriate.
The benchmark descriptions will be posted on the MC 2020 website. Furthermore, the organizers are considering publishing the collection of system and benchmark descriptions on arxiv.
Please submit benchmarks by email to [benchmarks@mccompetition.org](mailto:benchmarks@mccompetition.org) using the subject title "MC 2020 benchmark submission" by *March 5 AoE* the latest.


## Call for Participation

- DIMACS-based submission formats as given at the [competition format description](mc_format).

#### Registration
1. Register at optil.io (<https://www.optil.io/optilion/login>)
2. Access Easychair (mc2020, <https://easychair.org/conferences/?conf=mc2020>) and register your group 
   - Use as title of the paper your login name at optil
   - Place the name of your solver in the abstract
3. Optional: Test the formats of your solution via optil for [Model Counting](https://www.optil.io/optilion/problem/3183), [Weighted Model Counting](https://www.optil.io/optilion/problem/3184) and [Projected Model Counting](https://www.optil.io/optilion/problem/3185)
4. __Regularly submit your solution via optil for [Model Counting](https://www.optil.io/optilion/problem/3186) and [Weighted Model Counting](https://www.optil.io/optilion/problem/3187)__


#### Requirements
1. As programming languages we plan to allow C, C++, C#, Java8, Java10, Python2, Python3, Rust, and VB.NET. 
2. Open Source (e.g. GPL, MIT, or public domain)
3. Source code is available on a public repository (e.g., [Bitbucket](https://bitbucket.org), [GitHub](https://github.com), [Gitlab](https://gitlab.com)).
**Note:** We allow a limited use of external dependencies. These external dependencies may include commercial solvers such as [IBM Cplex](http://www-01.ibm.com/software/integration/optimization/cplex-optimizer), [gurobi](https://www.gurobi.com/), as well as open source solvers. 
 However, please contact us in advance, since we need to get it running on optil.io. 
4. Submissions Solver: Deadline (DS)
   1. Submission via [optil.io](https://www.optil.io/optilion/)
   2. Register solver and participants via [EasyChair](https://easychair.org/conferences/?conf=TBA)
   3. Create a release in the public repository of the solver (name: mc-2020)
5. Submission Description: Deadline (DD)
   1. Place the source code of the solver in a digital library (e.g., [Zenodo](https://zenodo.org/)) and generate a DOI 
   2. Submit solver description via [EasyChair](https://easychair.org/conferences/?conf=TBA) use DOI to refer to the solver and include a reference to the public source code repository 
<!--For parallel solving on GPUs, we aim for Nvidia cuda.-->


#### Optil System
1. Check [Optil Environment](https://www.optil.io/optilion/environment) and [Optil Help](https://www.optil.io/optilion/help)
2. Optil runs on a Xenial; benchmarks are run in a docker container
3. Restrictions/Runtime limitations:
- Runtime: 900s (soft cpu), 905 (hard cpu), 1000 (soft wall), 1005 (hard wall)
- Output: 524288 B
- Mem: 8,388,608 KB


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
