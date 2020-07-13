---
---

# MC 2020 (Model Counting 2020)

## How to use Optil.io?
We refer to a [more detailed subpage](optil).


## Tracks / Challenges
1. *Model Counting (mc)*
(Compute the number of satisfying assignments to a given CNF):<br/>
[Details for the track (Formats)](mc_format#track-1-model-counting)<br/>
[Optil Test Submission (Lite Track / allows to test your parser etc...)](https://www.optil.io/optilion/problem/3183)<br/>
[Optil Track Submission](https://www.optil.io/optilion/problem/3186)<br/>
[Download Public Instances (available now: 2020-04-21)](/assets/files/2020/mcc2020_track1-mc_public.tar);
[Download Private Instances (available now: 2020-07-13)](https://cloudstore.zih.tu-dresden.de/index.php/s/86A6TdJweCRixKs);
[Download All Instances (available now: 2020-07-13)](https://cloudstore.zih.tu-dresden.de/index.php/s/SNwJiP4MZxsZE94);

2. *Weighted Model Counting (wmc)*
(Compute the number of satisfying assignments to a given CNF):<br/>
[Details for the track (Formats)](mc_format#track-2-weighted-model-counting)<br/>
[Optil Test Submission (Lite Track / allows to test your parser etc...)](https://www.optil.io/optilion/problem/3184)<br/>
[Optil Track Submission](https://www.optil.io/optilion/problem/3187)<br/>
[Download Public Instances (Updated: 2020-05-03)](/assets/files/2020/mcc2020_track2-wmc_public.tar);
[Download Private Instances (available now: 2020-07-13)](https://cloudstore.zih.tu-dresden.de/index.php/s/tFn6qoa5tWKEtaY);
[Download All Instances (available now: 2020-07-13)](https://cloudstore.zih.tu-dresden.de/index.php/s/2K86Qzj2NBJGySM);


3. *Projected Model Counting (pmc)*
(Compute the number of satisfying assignments to a given CNF):<br/>
[Details for the track (Formats)](mc_format#track-3-projected-model-counting)<br/>
[Optil Test Submission (Lite Track / allows to test your parser etc...)](https://www.optil.io/optilion/problem/3185)<br/>
[Optil Track Submission (TBA)](https://www.optil.io/optilion/problem/3188)<br/>
[Download Public Instances (available now: 2020-06-03)](https://cloudstore.zih.tu-dresden.de/index.php/s/Zgn6eD7NYokNgct);
[Download Private Instances (available now: 2020-07-13)](https://cloudstore.zih.tu-dresden.de/index.php/s/mtmLXeBSSLzW5SN);


## Competition
The _1st International Competition on Model Counting (MC 2020)_ is a competition to deepen the relationship between latest theoretical and practical development on the various model counting problems and their practical applications. It targets the problem of counting the number of models of a Boolean formula. 

## Background
The success of solver technologies for declarative languages, such as SAT, in the last two decades is mainly due to both the availability of numerous efficient solver implementations and to the growing number of problems that can efficiently be solved through the declarative approach. Designing efficient solvers requires both understanding of the fundamental algorithms underlying the solvers, as well as in-depth insights into how to implement the algorithms for obtaining efficient and robust solvers.

Several competitive events are regularly organized for different declarative solving paradignms, including SAT competitions QBF evaluations, MaxSAT evaluations, SMT, ASP and CP competitions, etc., to evaluate available solvers on a wide range of problems. The winners of such events set regularly new standards in the area. If the systems themselves are widely spread, many details on their design or in their implementation can only be found in the source code of the systems.

The aim of the workshop is to allow researchers to share both fundamental theoretical insights into practical solvers, as well as new implementation-level insights and 'gory' technical details about their systems that may at times be difficult to publish in the main conferences on the declarative solving paradigms.




MC 2020 aims to identify new challenging benchmarks and to promote new solvers for the problem as well as to compare them with state-of-the-art solvers. The MC 2020 follows a direction in the community of constraint solving, where already many competitions have been organized such as on [ASP](https://sites.google.com/view/aspcomp2019/) (7 editions), [CSP](http://xcsp.org/competition) (19 editions), [SAT](http://sat-race-2019.ciirc.cvut.cz/) (19 editions), [SMT](https://smt-comp.github.io/2019/) (14 editions), [MaxSAT](https://maxsat-evaluations.github.io/2019/) Evaluation (13 editions), [QBF](http://www.qbflib.org/) (8 editions).

For competition details, we refer <!--to the [Tracks of MC 2020](model-counting-competition.md) and--> to the [Submission Information](mc_submission).

## Model Counting

<!-- ---

## Field of Research -->

Model counting is very vibrant field that provided both recent advances in theory as well as in practical solving including various applications. State-of-the-art SAT or WMC (weighted model counting) search engines so far rely on standard techniques from SAT-based solving, knowledge compilation, or approximate solving by means of sampling using SAT solvers. There have been also successful implementations for parallel and distributed computation as well as massively parallel computation approaches. 

For further details on the problem, we refer to the [page on model counting](about).

<!-- Beside the theoretical research there are many implementations available, just to name some state of the art solvers, c2d, d4, DSHARP, miniC2D, cnf2eadt, bdd_minisat_all, and sdd (based on knowledge compilation techniques); ApproxMC4, and sts (based on approximate counting or sampling); Cache, sharpCDCL4, and sharpSAT (CDCL-based solvers using component caching); gpusat, countAntom, and dCountAntom) (parallel or distributed solvers). There are also preprocessors available B+E and pmc. Many solvers are highly competitive and solve various instances. However, there has still not been a competition on the topics related to model counting.  -->

---


<!-- # Sponsors -->



<!-- # Previous Work

Previous simulations included works on the [Turing](https://www.cs.uni-potsdam.de/bs/research/labs.html#turing) and [Zuse](https://www.cs.uni-potsdam.de/bs/research/labsZuse.html) Cluster at University of Potsdam for various projects. As well as various clusters at TU Wien, more detailed, [Behemoth](https://www.ac.tuwien.ac.at/students/), Cobra, which Markus and I helped to congure for operations, and Lion used for the ASP'14 Competition at FLoC Clusters. In addition, we contributed to [benchmark-tools](https://github.com/potassco/benchmark-tool), which allow reproducibility of benchmarks under various cluster schedulers. Finally, Markus Hecher and I were organizers of the 4th Parameterized Algorithms and Computational Experiments Challenge (PACE 2019).

--- -->

## Organization

### Program Co-Chair
* Markus Hecher (TU Wien, Vienna)
* Johannes K. Fichte (TU Dresden, Dresden)

### Student
* Florim Hamiti (TU Dresden, Dresden)

### Scientific Partners
* Adnan Darwiche (University of California at Los Angeles)
* Arthur Choi (University of California at Los Angeles)
* Armin Biere (Johannes Kepler Universitat Linz)
* Kuldeep S. Meel (National University of Singapore)
* Markus Hecher (TU Wien)
* Johannes K. Fichte (TU Dresden)
* Marijn Heule (Carnegie Mellon University)
* Norbert Manthey
* Stefan Mengel (CNRS at Centre de Recherche en Informatique de Lens)
* Pierre Marquis (CNRS at Centre de Recherche en Informatique de Lens and Université d'Artois)
* Fahim Bacchus (University of Toronto)
* Vibhav Gogate (University of Texas at Dallas)

### Evaluation Plattform / optil.io
Szymon Wasik (Poznan University of Technology, Poznan)

## Sponsors


On behalf of the Program Committee of MC 2020, we invite you to participate in the sponsoring of metals and travel support for the winners.


[data-experts](https://data-experts.de) already announced sponsoring for MC 2020.

<img src="../assets/images/data-experts-logo.png" alt="data-experts" style="width: 300px;"/>

---
