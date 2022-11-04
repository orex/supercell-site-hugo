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

The benchmark which was published in the supercell paper (PbSnTe<sub>2</sub> 2x2x2) is obsolete. The current version of supercell program can process the configuration in a few seconds. More important that this test do nothing useful. Therefore below, I'll use more advanced test case with 10<sup>11</sup> total number of combinations, which does "wet-run" and generates output structures with random sampling and the lowest electrostatic energy. This is a real practical case of using of `supercell` program. The input file can be downloaded from supercell distribution [CaAl6Te10.cif](https://raw.githubusercontent.com/orex/supercell/master/data/examples/CaAl6Te10/CaAl6Te10.cif).

**Test command**
```
supercell -i CaAl6Te10.cif -m -q -n r10 -n l10 -v 2
```

The tests were run ones for each of such configurations:

*   Intel® Xeon® Gold 6226R 2.90GHz CPU (32 cores).
*   Ubuntu 16.04 LTS
*   Binary files from supercell site.

During this run 10<sup>11</sup> structures process in 117 and 6 minutes on 1 and 32 cores respectively. The maximum performance is around 300 mln structures per second.

#### Scalability

Some test were performed to check scalability property of the program (see figure below). The y-axis shows performance per core normalized to performance v2.1 on one core. The extrapolation shows that even 64 cores can decrease processing time, because it is still higher than saturation limit.

![image](/supercell/images/scalable-plot.svg)

#### Optimal performance recommendations
   
* Use Linux. Other platforms binaries are not so well optimized as Linux binary.
* Optimal compiling of supercell program requires advanced programming skills, so binaries from the site is OK for most of the users.
* Supercell performance is very good correlated with benchmark scores from [cpubenchmark.net](https://www.cpubenchmark.net/). You can use the data to find optimal solution for running the program. 
