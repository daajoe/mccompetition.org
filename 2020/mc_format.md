---
---
# MC-2020 Competition Format
## Track 1: Model Counting

Solver submissions for this track should output for a given Boolean formula
the model count of the instance.

### Input Instance Format

Input files are given in [DIMACS CNF format](https://people.sc.fsu.edu/~jburkardt/data/cnf/cnf.html).

#### DIMACS CNF (.cnf)

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
c This file describes that the model count is 30
s mc 30
```


### Instances

TBA

<!--Download: [**Download (Updated: March 05, 2019) Public Instances (Exact)**](/files/pace2019-vc-exact-public-v2.tar.bz2)-->

<!--For verification purposes, we also publish the sha1sum of the public archive:-->

<!--SHA1 sum | filename 
--- | --- 
e7ca305528a0257235a95c41742f2b3431e1e485  | pace2019-vc-exact-public-v2.tar.bz2-->

<!--For individual files we refer to [Download SHA1 sums](/files/pace2019-vc-exact-public-shasums-v2.txt)-->


---


## Track 2: Weighted Model Counting 

Solver submissions for this track should output for a given Boolean formula,
and a weight function, the weighted model count of the instance.

### Input Instance Format

Input files are given in _Weighted CNF format_, which is a slight extension of [DIMACS CNF format](https://people.sc.fsu.edu/~jburkardt/data/cnf/cnf.html).

#### Weighted CNF (.wcnf)

* Format as DIMACS CNF
* Line separator ‘\n’
* Lines starting with character c are interpreted as comments
* Variables are consecutively numbered from 1 to n
* Problem description
  * Form "p wcnf NumVariables NumClauses"
    * Line starting with character p 
    * followed by the problem descriptor cnf 
    * followed by number n of variables
    * followed by number m of clauses
    * each separated by space each time
  * Unique (No other line may start with p)
  * Has to be the first line (except comments)
* Weight function
  * Lines of the form "w Literal Weight 0"
  * Defines the floating point Weight for Literal, where 0 <= Weight <= 1 
  * We do not use more than 9 significant digits after the decimal point
  * If the weight for a literal is not defined, it is considered to be of weight 1
* Remaining lines indicate clauses
  * consisting of decimal integers separated by space
  * Lines are terminated by character "0"
  * Line "2 -1 3 0\n" indicates the clause "2 or not 1 or 3"
* Empty lines or lines consisting of spaces may occur and only will be ignored  

Example:

```AsciiDoc
c This file describes a weighted CNF in MC 2020 format with 6 variables and 4 clauses 
p wcnf 6 4
w 1 0.4 0
w -1 0.6 0
w 4 0.5 0
w -4 0.5 0
w 5 1.0 0
w -5 1.0 0
-1 -2 0
2 3 -2 0
c this is a comment and will be ignored
4 5 0
4 6 0
```

### Output Format (.wmc)

* Line separator ‘\n’
* Lines starting with character c are interpreted as comments
* Vertices are consecutively numbered from 1 to n
* Solution description
  * Form "s wmc numSolutions"
    * Line starting with character s
    * followed by the problem descriptor wmc 
    * followed by number numSolutions indicating the weighted model count
    * each separated by space each time
  * Unique (No other line may start with s)
  * Has to be the first line (except comments)
* Empty lines or lines consisting of spaces may occur and only will be ignored  


```AsciiDoc
c This file describes that the weighted model count is 8.0
s wmc 8.0
```



## Track 3: Projected Model Counting 

Solver submissions for this track should output, for a given Boolean formula
and set of projection variables, the projected model count of the instance.


### Input Instance Format

Input files are given in _Projected CNF format_, which is a slight extension of
 [DIMACS CNF format](https://people.sc.fsu.edu/~jburkardt/data/cnf/cnf.html).

#### Projected CNF (.pcnf)

* Format as DIMACS CNF
* Line separator ‘\n’
* Lines starting with character c are interpreted as comments
* Variables are consecutively numbered from 1 to n
* Problem description
  * Form "p pcnf NumVariables NumClauses"
    * Line starting with character p 
    * followed by the problem descriptor cnf 
    * followed by number n of variables
    * followed by number m of clauses
    * followed by number of projected variables
    * each separated by space each time
  * Unique (No other line may start with p)
  * Has to be the first line (except comments)
* Set of projected variables 
  * Line of the form "vp VARID1 VARID2 VARID3 0"
  * Unique (No other line may start with vp)
  * Line may occur at any time after the p line, esp. also as last line in the file
  * Defines the projected variables, i.e., variables that are important and which are the ones that _will_ be considered for the count
  * Consisting of decimal integers separated by space
  * Lines are terminated by character "0"
  * Line "vp 1 2 0\n" indicates the set {1, 2} of projection variables
  * 1 <= VARID <= n (n... number of variables)   
* Remaining lines indicate clauses
  * consisting of decimal integers separated by space
  * Lines are terminated by character "0"
  * Line "2 -1 3 0\n" indicates the clause "2 or not 1 or 3"
* Empty lines or lines consisting of spaces may occur and only will be ignored  

Example:

```AsciiDoc
c This file describes a projected CNF in MC 2020 format with 6 variables and 4 clauses and 2 projected variables 
p pcnf 6 4 2
vp 1 2 0
-1 -2 0
2 3 -2 0
c this is a comment and will be ignored
4 5 0
4 6 0
```

### Output Format (.pmc)

* Line separator ‘\n’
* Lines starting with character c are interpreted as comments
* Vertices are consecutively numbered from 1 to n
* Solution description
  * Form "s pmc numSolutions"
    * Line starting with character s
    * followed by the problem descriptor pmc 
    * followed by number numSolutions indicating the projected model count
    * each separated by space each time
  * Unique (No other line may start with s)
  * Has to be the first line (except comments)
* Empty lines or lines consisting of spaces may occur and only will be ignored  


```AsciiDoc
c This file describes that the projected model count is 3
s pmc 3
```

---

