---
title: "Benchmark"
draft: false
icon: 
type: "docs"
card:
  order: 6
  description: "The supercell program is the fastest solution which can approach the largest enumeration problems."
  btncaption: "Check the results"
  btnicon: "fas fa-tachometer-alt"
  highlighted: false
---

#### Results

The same benchmark as in supercell paper (the same as fcc in disorder paper). Time in seconds. "Binaries" are compiled program which is available on this site, "native" program was built to run optimally on the test machine.

The tests were run ones each on such configuration:

*   KVM Intel® Xeon® 3.1 GHz (8 cores).
*   Ubuntu 20.04 LTS
*   "Native" executables were built with default compilers, build-toolchain etc in Ubuntu 20.04. OpenBabel 2.4.x version vere used for v1.2
*   Test command line: `supercell -i PbSnTe2.cif -m -d -s 2x2x2`

<div class="container-fluid col-lg-10 col-md-12 col-sm-12 col-xs-12">
  <table class="table">
    <thead class="table-light">
    <tr>
      <th scope="col">Configuration</th>
      <th scope="col">binaries</th>
      <th scope="col">native</th>
    </tr>
    </thead>
    <tbody>
    <tr>
      <th scope="row">v1.2 (1 core)</th>
      <td>372.28</td>
      <td>307.58</td>
    </tr>
    <tr>
      <th scope="row">v2.0 (1 core)</th>
      <td>32.93</td>
      <td>32.65</td>
    </tr>
    <tr>
      <th scope="row">v2.0 (8 cores)</th>
      <td>12.27</td>
      <td>14.62</td>
    </tr>
    </tbody>
  </table>
</div>

Compiled v1.2 shows slower performance due to compatibility with very old platforms. Surprisingly slower performance of "native" binaries with 8 cores can be most probably explained by previous version of TBB library from Ubuntu repository, which was used for compiling the code.

#### Recommendations

Some recommendation for optimal supercell performance:

*   Use Linux.
*   Prefer to run supercell on modern Workstation/Desktop rather than on old HPC.
*   The example above is a "special" example which is used to compare different enumeration approaches. It does not include practical aspects like sampling. Please, use more real-world scenarios to check supercell code performance. For example `supercell -i data/examples/CaAl6Te10/CaAl6Te10.cif -m -q -n r10 -n l10 -v 2` run includes electrostatic calculation and random sampling, which is needed in almost all practical cases. During this run 10<sup>11</sup> structures process in 137 and 28 minutes on 1 and 8 threads respectively on Intel® Xeon® Gold 6226R 2.90GHz CPU.
*   For regular users binaries are a preferable option. Now, with drop of old platforms support, they show a good performance. If you would like to install *supercell* on cluster, try to compile it by yourself with different compilers and options. Probably Intel compiler can improve the program performance.
