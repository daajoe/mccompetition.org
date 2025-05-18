# Submission Instructions

All tracks will be run on the [BenchCloud Instance of SoSy Lab in Munich](https://benchcloud.sosy-lab.org/) using compute nodes with an 8 cores Intel Xeon E3-1230 v5 @ 3.40 GHz CPU. The solvers will be executed with a time limit of 3600 seconds and memory limit of 32GB.

## Testing and Requirements

The solver should be able to be built and run on a system that conforms to the specification in the [Computing Environment on Competition Machines](https://gitlab.com/sosy-lab/benchmarking/competition-scripts/#computing-environment-on-competition-machines) section of the SoSy Lab Competition Scripts. The top-level directory of your solver should contain two scripts:

- **build.sh**, for building the counter.
  The build script should take no parameters and should be tested and work on the provided Docker image.

- **run.sh**, to run the counter.
  The run script should take only one parameter: the path to the benchmark instance. The output should follow the [format document](../../assets/files/mccomp_format_24.pdf) and should be written to stdout.



## Submission

The submission of the final version of a solver is via a private GitHub repository, which is to be made available to the organizers by the solver authors.

### Emailing your System Description Document

After you have submitted the final version of your solver, send an email to the organizers (mcw at modelcounting.org) containing your system description document (see General Rules for more information).
