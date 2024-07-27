---
---

# Workshop on Counting, Sampling, and Synthesis 2024

## Registration

Please register for the SAT conference.

## Purpose

The _Workshop on Counting, Sampling, and Synthesis_ is an event for researchers in model counting and sampling. It covers advanced topics such as weighted and projected counters/samplers and various domains such as SAT, SMT, ASP, and CP. This year, the workshop has expanded its focus to include the role of model counters, samplers, and solvers in automated synthesis. The goal of the workshop is to facilitate the exchange of cutting-edge theoretical and practical insights, with a particular emphasis on innovative solver technologies and their real-world applications. Additionally, the workshop provides an opportunity for developers of model counters to showcase their work and share detailed competition results, to encourage discussions that bridge theory and practice.

## Venue

This year’s event will be held alongside other workshops at the SAT 2024 conference. For more information, please visit the [SAT 2024 website](http://satisfiability.org/SAT24/venue.php).

## Accepted Talks

<style>
td, th {
    border: 1px solid grey
}
table th:first-of-type {
    width: 50%;
}
table th:nth-of-type(2) {
    width: 50%;
}
</style>

| Title | Author(s)|
|-------|:---------|
|Exact ASP Counting with Compact Encodings <details> Answer Set Programming (ASP) has established itself as a robust paradigm for knowledge representation and automated reasoning, adept at handling complex combinatorial problems across various domains. Leveraging developments in propositional SAT solving, the last two decades have seen the advent of sophisticated systems capable of addressing the answer set satisfiability problem, which involves identifying models or answer sets for specific ASP programs. Recently, interest has expanded to include more complex problems, such as model counting within ASP. This work introduces a novel framework for ASP counting, named sharpASP, designed to efficiently count answer sets without heavyweight propositional encoding. It employs an innovative approach to defining answer sets, incorporating advanced techniques from propositional model counting. Our comprehensive empirical evaluation, involving 1470 benchmarks, reveals that sharpASP significantly outperforms existing exact answer set counters. Specifically, sharpASP resolved 1062 benchmarks with a PAR2 score of 3082, compared to the previous best of 895 benchmarks with a PAR2 score of 4205 under identical experimental conditions. </details> |  Mohimenul Kabir, Supratik Chakraborty and Kuldeep S Meel |
|An Approximate Skolem Function Counter <details>Motivated by the recent development of scalable approaches to Boolean function synthesis, we study the following problem: Given a Boolean specification between a set of inputs and outputs, count the number of functions of inputs such that the specification is met. Counting Skolem functions poses considerable new challenges. From the complexity-theoretic standpoint, counting Skolem functions is not only #P -hard; it is quite unlikely to have an FPRAS as the problem of synthesizing a Skolem function remains challenging, even given access to an NP oracle. The primary contribution of this work is the first algorithm, SkolemFC, that computes an estimate of the number of Skolem functions. SkolemFC relies on technical connections between counting functions and propositional model counting: our algorithm makes a linear number of calls to an approximate model counter and computes an estimate of the number of Skolem functions with theoretical guarantees. Moreover, we show that Skolem function count can be approximated through a polynomial number of calls to a SAT oracle. Our prototype displays impressive scalability, handling benchmarks comparably to state-of-the-art Skolem function synthesis engines, even though counting all such functions ostensibly poses a greater challenge than synthesizing a single function. </details> | Arijit Shaw, Kuldeep S. Meel and Brendan Juba|
|Proof Systems for Tensor-based Model Counting <details> The model counting problem #SAT, asking for the number of satisfying assignments of a propositional formula, has been explored intensively in the #SAT solving community. One of the main algorithmic approaches for #SAT solving is through contraction in tensor hypernetworks. We perform a theoretical proof-complexity analysis of this approach. For this, we design two new tensor-based proof systems that we show to tightly correspond to tensor-based #SAT solving. We determine the simulation order of #SAT proof systems and prove exponential separations between the systems. This sheds light on the relative performance of different #SAT solving approaches.</details> | Olaf Beyersdorff, Joachim Giesen, Andreas Goral, Tim Hoffmann, Kaspar Kasche and Christoph Staudt| |
|Circuits, Proofs and Propositional Model Counting <details> In this paper we present a new proof system framework CLIP (Circuit Linear Induction Proposition) for propositional model counting.A CLIP proof firstly involves a circuit, calculating the cumulative function (or running count) of models counted up to a point, and secondly a propositional proof arguing for the correctness of the circuit. This concept is remarkably simple and CLIP is modular so allows us to use existing checking formats from propositional logic, especially strong proof systems. Despite model counting being a harder problem than unsatisfiability, we find that CLIP only has lower bounds from its propositional proof system or if P^{#P} is not contained in P/poly, similar to results in QBF proof complexity (Beyersdorff et al. Journal of the ACM 2020). From a proof complexity point of view we find it is exponentially stronger than existing proof systems MICE (Fichte et al. SAT 2022) and KCPS(#SAT) (Capelli SAT 2019) for propositional model counting.</details>  | Sravanthi Chede, Leroy Chew and Anil Shukla |
|Testing Self-Reducible Samplers <details> Samplers are the backbones of randomized algorithms. Unfortunately, obtaining an efficient algorithm to test the correctness of samplers is very hard. Recently, in a series of works, testers like Barbarik, Teq, and Flash for testing some particular samplers, such as Cnf-samplers, were developed. However, their techniques have significant limitations because one cannot expect to use their methods to test other samplers, such as samplers for graphs. In this paper, we present a new testing algorithm that works for such samplers and can estimate the distance of a target sampler from an ideal sampler (say, uniform sampler). This paper's main contribution is a new distance estimation algorithm for distributions over high-dimensional cubes using the recently proposed sub-cube conditioning model. Given subcube conditioning access to an unknown distribution, and a known distribution defined over n dimensional hypercube, our algorithm estimates the variation distance between the distributions within an additive error. The estimation algorithm in the sub-cube conditioning model helps us to design the first tester for self-reducible samplers. We also implement our algorithm and use it to test the quality of three state-of-the-art graph samplers.</details> | Rishiraj Bhattacharyya, Sourav Chakraborty, Yash Pote, Uddalok Sarkar and Sayantan Sen |
|Formally Certified Approximate Model Counting <details>Approximate model counting is the task of approximating the number of solutions to an input Boolean formula. The state-of-the-art approximate model counter for formulas in conjunctive normal form (CNF), ApproxMC, provides a scalable means of obtaining model counts with probably approximately correct (PAC)-style guarantees. Nevertheless, the validity of ApproxMC's approximation relies on a careful theoretical analysis of its randomized algorithm and the correctness of its highly optimized implementation. We present the first certification framework for approximate model counting with formally verified guarantees on the quality of its output approximation. Our approach combines: (i) a static, once-off, formal proof of the algorithm's PAC guarantee in the Isabelle/HOL proof assistant; and (ii) dynamic, per-run, verification of ApproxMC's calls to an external CNF-XOR solver using proof certificates. We detail our general approach to establish a rigorous connection between these two parts of the verification, including our blueprint for turning the formalized, randomized algorithm into a verified proof checker, and our design of proof certificates for both ApproxMC and its internal CNF-XOR solving steps. Experimentally, we show that certificate generation adds little overhead to an approximate counter implementation, and that our certificate checker is able to fully certify 84.7\% of instances with generated certificates.</details> | Yong Kiam Tan, Jiong Yang, Mate Soos, Magnus O. Myreen and Kuldeep S. Meel |



## Schedule

Coming soon..

<!---

## Timeline

See [Dates](dates).

## Format

You can showcase your best work in counting, sampling, or synthesis, whether it has been published elsewhere or not. Presenters can choose between giving a talk or presenting a poster. Each talk will have a 20-minute time slot for the presentation, followed by a 10-minute Q&A session.

## Submissions

- **Submission.** There are no specific format requirements. We expect you to provide a reasonable description in PDF format and upload it on [EasyChair](https://easychair.org/conferences/?conf=mcw2024).
- **Procedure for selecting papers.** All submissions will be reviewed by 1-2 program committee members, who will make recommendations for paper selection. If there are too many talk submissions, some authors may be requested to present a poster instead.
- **Plans for dissemination.** There will be no proceedings, but the abstracts and slides will be made available on the website. If authors decide to prerecord a video, it will be shared with the participants.

-->

## Contact

If you have any questions about the workshop, the best way to contact the organizers is by emailing <span style="color:blue">mcw at modelcounting.org</span>.

## Team

### Organizers

- [Paulius Dilkas](https://dilkas.github.io) (University of Toronto, Canada)
- [Priyanka Golia](https://priyanka-golia.github.io) (Indian Institute of Technology Delhi, India)

### Steering Committee

- [Johannes K. Fichte](https://liu.se/en/employee/johfi52) (Linköping University, Sweden)
- [Markus Hecher](https://dbai.tuwien.ac.at/staff/hecher/) (Massachusetts Institute of Technology, USA)
- [Kuldeep S. Meel](https://www.cs.toronto.edu/~meel/) (University of Toronto, Canada)

---
