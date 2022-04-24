---
title: "Background"
description: "Introduction to supercell program."
draft: false
---

A supercell approach is a very old, universal and theoretically clean method for approximation of materials with point disorder[^1]. But the method applies mostly to some particular cases, like low amount of impurity (one per supercell) or random disorder with special quasirandom structure (SQS) approximation[^2], because the number of derivative structures is one in these cases. In general, the number of derivative structures is high enough to be generated "by hand". There are some programs, which can help to generate derivative structures (see [review](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-016-0129-3#Sec14)). We believe that supercell program is the best choice, because the software was created to solve most of the technical problems of supercell approximation. The program includes algorithms for structure manipulation, supercell generation, permutations of atoms and vacancies, charge balancing, detecting symmetry-equivalent structures, electrostatic energy calculations and sampling output derivative structures. The software works with CIF files, therefore it is compatible with most of DFT software ([VASP](http://www.vasp.at/), [CASTEP](http://www.castep.org/), [Wien2k](http://wien2k.at/) etc). It has a powerful command line interface and works out-of-the-box on Linux, macOS and Windows platforms. The correctness of the program was verified by available literature data. The documentation includes open access paper, program interface manual, tutorial and variety of examples.

[^1]: Buerger, M. J. (1947). J. Chem. Phys., 15(1), 1–16.
[^2]: Zunger, A., Wei, S. H., Ferreira, L. G., & Bernard, J. E. (1990). PRL, 65(3), 353–356.
