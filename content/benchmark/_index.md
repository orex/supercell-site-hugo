---
title: "Benchmark"
date: 2022-04-12T11:11:11+06:00
draft: false
type: "docs"
weight: 70
card:
  order: 6
  description: "The supercell program is the fastest solution which can approach the largest enumeration problems."
  btncaption: "Check the results"
  btnicon: "fas fa-tachometer-alt"
  highlighted: false
---

#### Results

The benchmark which was published in the supercell paper (PbSnTe<sub>2</sub> 2x2x2) is obsolete. The current version of supercell program can process the configuration in a few seconds. More importantly, this test does nothing useful. Therefore, below I use a more advanced test case with 10<sup>11</sup> total combinations, which does a "wet-run" and generates output structures with random sampling and the lowest electrostatic energy. This is a real practical case of using the `supercell` program. The input file can be downloaded from supercell distribution [CaAl6Te10.cif](https://raw.githubusercontent.com/orex/supercell/master/data/examples/CaAl6Te10/CaAl6Te10.cif).

**Test command**
```
supercell -i CaAl6Te10.cif -m -q -n r10 -n l10 -v 2
```

The tests were run once for each of the configurations below:

*   Intel® Xeon® Gold 6226R 2.90GHz CPU (32 cores).
*   Ubuntu 16.04 LTS
*   Binary files from supercell site.

During this run 10<sup>11</sup> structures were processed in 117 and 6 minutes on 1 and 32 cores respectively. The maximum performance is around 300 mln structures per second.

#### Scalability

Some tests were performed to check the scalability of the program (see figure below). The y-axis shows performance per core normalized to v2.1 performance on one core. The extrapolation shows that even at 64 cores adding more cores still decreases processing time, because per-core performance is still above the saturation limit.

![image](/supercell/images/scalable-plot.svg)

#### Optimal performance recommendations
   
* Use Linux. Binaries for other platforms are not as well optimized as the Linux binary.
* Optimal compiling of supercell program requires advanced programming skills, so binaries from the site are OK for most users.
* Supercell performance correlates very well with benchmark scores from [cpubenchmark.net](https://www.cpubenchmark.net/). You can use that data to find an optimal solution for running the program.
