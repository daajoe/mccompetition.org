---
bibliography: references.bib
---

# List of Solvers

## Model Counting (MC)

| Solver          | Execution | Technique | Target  | Reference                      | Download                                                                   | License |
|:----------------|:----------|:----------|:--------|:-------------------------------|:---------------------------------------------------------------------------|:--------|
| ADDMC           | SEQ       | DP        | PTW+ADD | DudekPhanVardi20b              | [Sources](https://github.com/vardigroup/ADDMC)                             | MIT     |
| ApproxMC        | SEQ       | AC        |         | ChakrabortyEtAl14a             | [Sources](https://github.com/meelgroup/approxmc)                           | MIT     |
| bdd_minisat_all | SEQ       | BDD       |         | TodaSoh15a                     | [Sources](http://www.sd.is.uec.ac.jp/toda/code/cnf2obdd.html)              | MIT     |
| c2d             | SEQ       | KC        | d-DNNF  | Darwiche04a                    | [Binaries](http://reasoning.cs.ucla.edu/c2d/download.php)                  | na      |
| Cachet          | SEQ       | CC        |         | SangEtAl04                     | [Sources](https://www.cs.rochester.edu/u/kautz/Cachet/cachet-wmc-1-21.zip) | zchaff  |
| cnf2eadt        | SEQ       | KC        | EADT    | KoricheLagniezMarquisThomas13a | [Binaries](http://www.cril.univ-artois.fr/KC/eadt.html)                    | na      |
| d4              | SEQ       | KC        | d-DNNF  | LagniezMarquis17a              | [Sources](https://github.com/crillab/d4)                                   | na      |
| DPMC            | SEQ       | DP        | PTW     | DudekPhanVardi20a              | [Sources](https://github.com/vardigroup/DPMC)                              | MIT     | 
| DSHARP          | SEQ       | KC        | d-DNNF  | MuiseEtAl12a                   | [Sources](https://github.com/QuMuLab/dsharp)                               | GPL2    |
| Ganak           | SEQ       | CC        |         | SharmaEtAl19a                  | [Sources](https://github.com/meelgroup/ganak)                              | MIT     |
| GPMC            | SEQ       | CC        |         | na                             | [Sources](https://git.trs.css.i.nagoya-u.ac.jp/k-hasimt/GPMC)              | MIT     | 
| miniC2D         | SEQ       | KC        | SDD     | OztokDarwiche15a               | [Binaries](http://reasoning.cs.ucla.edu/minic2d/)                          | na      |
| mcTW            | SEQ       | DP        |         | na                             | [Sources](https://github.com/swacisko/mc-2020)                             | MIT     |
| ProCount        | SEQ       | DP        | PTW     | DudekPhanVardi21               | [Sources](https://github.com/vardigroup/DPMC)                              | MIT     |
| riss            | SEQ       | CC        |         |                                | [Sources](https://github.com/nmanthey/riss-solver)                         | LGPL    |
| sdd             | SEQ       | KC        | SDD     | Darwiche11a                    | [Binaries](http://reasoning.cs.ucla.edu/sdd/)                              | na      |
| sharpCDCL       | SEQ       | CC        |         | na                             | [Sources](https://github.com/conp-solutions/sharpCDCL)                     | GPL2    |
| sharpSAT        | SEQ       | CC        |         | Thurley06a                     | [Sources](https://github.com/marcthurley/sharpSAT)                         | MIT     |
| SharpSAT-TD     | SEQ       | CC        |         | KorhonenJarvisalo21            | [Sources](https://github.com/Laakeri/sharpsat-td)                          | MIT     |
| SUMC            | SEQ       | DP        | PTW     | na                             | [Sources](https://github.com/ivor-spence/sumc)                             | GPL3    |
| sts             | SEQ       | AC        |         | ErmonGomesSelman12a            | [Sources](http://cs.stanford.edu/~ermon/code/STS.zip)                      | MIT     |
| countAntom      | PAR       | CC        |         | BurchardSchubertBecker15a      | [Sources](https://projects.informatik.uni-freiburg.de/projects/countantom) | MIT     |
| dpdb            | PAR       | DP        | PTW     | FichteEtAl20                   | [Sources](https://github.com/hmarkus/dp_on_dbs/tree/padl2020)              | GPL3    |
| nestHDB         | PAR       | DP        | ATW     | HecherThierWoltran20           | [Sources](https://github.com/hmarkus/dp_on_dbs/tree/nesthdb)               | GPL3    |
| gpusat          | PAR       | DP        | PTW/ITW | FichteHecherZisser19a          | [Sources](https://github.com/daajoe/GPUSAT)                                | GPL3    |
| gpusat-cuda     | PAR       | DP        | PTW     | FichteHecherRoland21           | [Sources](https://github.com/vroland/GPUSAT)                               | GPL3    |
| TensorOrder2    | PAR       | DP        |         | DudekVardi20                   | [Sources](https://github.com/vardigroup/TensorOrder)                       | MIT     |
| dCountAntom     | DIST      | CC        |         | BurchardSchubertBecker16a      | na                                                                         | na      |
| DMC             | DIST      | KC        | d-DNNF  | LagniezMarquisSzczepanski18a   | [Binaries](http://www.cril.univ-artois.fr/KC/dmc.html)                     | na      |

## Weighted Model Counting (WMC)

| Solver          | Execution | Technique | Target  | Reference                      | Download                                                                   | License |
|:----------------|:----------|:----------|:--------|:-------------------------------|:---------------------------------------------------------------------------|:--------|
| ADDMC           | SEQ       | DP        | PTW+ADD | DudekPhanVardi20b              | [Sources](https://github.com/vardigroup/ADDMC)                             | MIT     |
| Cachet          | SEQ       | CC        |         | SangEtAl04                     | [Sources](https://www.cs.rochester.edu/u/kautz/Cachet/cachet-wmc-1-21.zip) | zchaff  |
| c2d             | SEQ       | KC        | d-DNNF  | Darwiche04a                    | [Binaries](http://reasoning.cs.ucla.edu/c2d/download.php)                  | na      |
| d4              | SEQ       | KC        | d-DNNF  | LagniezMarquis17a              | [Sources](https://github.com/crillab/d4)                                   | na      |
| DPMC            | SEQ       | DP        | PTW     | DudekPhanVardi20a              | [Sources](https://github.com/vardigroup/DPMC)                              | MIT     | 
| Ganak           | SEQ       | CC        |         | SharmaEtAl19a                  | [Sources](https://github.com/meelgroup/ganak)                              | MIT     |
| gpusat          | PAR       | DP        | PTW/ITW | FichteHecherZisser19a          | [Sources](https://github.com/daajoe/GPUSAT)                                | GPL3    |
| TensorOrder2    | PAR       | DP        |         | DudekVardi20                   | [Sources](https://github.com/vardigroup/TensorOrder)                       | MIT     |
| miniC2D         | SEQ       | KC        | SDD     | OztokDarwiche15a               | [Binaries](http://reasoning.cs.ucla.edu/minic2d/)                          | na      |
| sts             | SEQ       | AC        |         | ErmonGomesSelman12a            | [Sources](http://cs.stanford.edu/~ermon/code/STS.zip)                      | MIT     |

## Projected Model Counting (PMC)

| Solver  | Execution | Technique | Target  | Reference            | Download                                                     | License |
|:--------|:----------|:----------|:--------|:---------------------|:-------------------------------------------------------------|:--------|
| ADDMC   | SEQ       | DP        | PTW+ADD | DudekPhanVardi20b    | [Sources](https://github.com/vardigroup/ADDMC)               | MIT     |
| d4      | SEQ       | KC        | d-DNNF  | LagniezMarquis17a    | [Sources](https://github.com/crillab/d4)                     | na      |
| DPMC    | SEQ       | DP        | PTW     | DudekPhanVardi20a    | [Sources](https://github.com/vardigroup/DPMC)                | MIT     |
| nestHDB | PAR       | DP        | ATW     | HecherThierWoltran20 | [Sources](https://github.com/hmarkus/dp_on_dbs/tree/nesthdb) | GPL3    |
| projMC  | SEQ       | KC        | d-DNNF  | LagniezMarquis19a    | [Binaries](http://www.cril.univ-artois.fr/KC/projmc.html)    | NA      |
| Ganak   | SEQ       | CC        |         | SharmaEtAl19a        | [Sources](https://github.com/meelgroup/ganak)                | MIT     |

## Projected Weighted Model Counting (PWMC)

| Solver | Execution | Technique | Target | Reference         | Download                                                      | License |
|:-------|:----------|:----------|:-------|:------------------|:--------------------------------------------------------------|:--------|
| DPMC   | SEQ       | DP        | PTW    | DudekPhanVardi20a | [Sources](https://github.com/vardigroup/DPMC)                 | MIT     |
| GPMC   | SEQ       | CC        |        | na                | [Sources](https://git.trs.css.i.nagoya-u.ac.jp/k-hasimt/GPMC) | MIT     | 





## Literature / References

[references.bib](../assets/files/references.bib)

---
