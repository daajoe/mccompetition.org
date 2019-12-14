---
---


# Competition Tracks

The challenge consists of two separate tracks: 
1. [Model Counting (MC)](about.md), and
2. [Weighted Model Counting (WMC)](about.md)

Note that we only allow non-parallel solvers.
For more details on active calls for benchmark instances and participation, 
we refer to [Submission & Important Dates](dates.md).

## Benchmark Instances

There will be 200 benchmark instances for each track, labeled (w)mc_001.dimacs to (w)mc_200.dimacs for the track on (W)MC, respectively. 
 
Larger numbers in the filename should (as a rule of thumb) correspond to harder instances. 
The odd instances are public and the even instances will be provided later (secret). 


## Evaluation 

- timeout: 30 minutes per instance
- measure: TBA; likely PAR-2, where timed-out runs are counted as 2 times the given timeout time.
- objective: minimize the measure


## Track 1: Model Counting

If the solver does not output the exact solution - the solver will not be disqualified, which ensures that we do not require arbitrary precision.

### Input Instance Format

Input files are given in [DIMACS CNF format](https://people.sc.fsu.edu/~jburkardt/data/cnf/cnf.html).

#### DIMACS CNF (.dimacs)

* Line separator ‘\n’
* Lines starting with character c are interpreted as comments
* Variables are consecutively numbered from 1 to n
* Problem description
  * Form "p cnf NumVariables NumClauses"
    * Line starting with character p 
    * followed by the problem descriptor cnf 
    * followed by number n of variables
    * followed by number m of clauses
    * each separated by space each time
  * Unique (No other line may start with p)
  * Has to be the first line (except comments)
* Remaining lines indicate clauses
  * consisting of decimal integers separated by space
  * Lines are terminated by character "0"
  * Line "2 -1 3 0\n" indicates the clause "2 or not 1 or 3"
* Empty lines or lines consisting of spaces may occur and only will be ignored  

Example:

```AsciiDoc
c This file describes a DIMACS CNF in MC 2020 format with 6 variables and 4 clauses 
p cnf 6 4
-1 -2 0
2 3 -2 0
c this is a comment and will be ignored
4 5 0
4 6 0
```

### Output Format (.mc)

* Line separator ‘\n’
* Lines starting with character c are interpreted as comments
* Vertices are consecutively numbered from 1 to n
* Solution description
  * Form "s mc numSolutions"
    * Line starting with character s
    * followed by the problem descriptor mc 
    * followed by number numSolutions indicating the model count
    * each separated by space each time
  * Unique (No other line may start with s)
  * Has to be the first line (except comments)
* Empty lines or lines consisting of spaces may occur and only will be ignored  


```AsciiDoc
c This file describes that the model count is 5
s mc 5
```


### Instances

TBA

<!--Download: [**Download (Updated: March 05, 2019) Public Instances (Exact)**](/files/pace2019-vc-exact-public-v2.tar.bz2)-->

<!--For verification purposes, we also publish the sha1sum of the public archive:-->

<!--SHA1 sum | filename 
--- | --- 
e7ca305528a0257235a95c41742f2b3431e1e485  | pace2019-vc-exact-public-v2.tar.bz2-->

<!--For individual files we refer to [Download SHA1 sums](/files/pace2019-vc-exact-public-shasums-v2.txt)-->

## Track 2: Weighed Model Counting

The solution does not have to be exact, but we expect 1% accuracy.


### Instances

TBA

---
