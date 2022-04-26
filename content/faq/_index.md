---
title: "Mostly Asked Questions"
date: 2022-04-12T11:11:11+06:00
type: "docs"
draft: false
weight: 50
---

### Does supercell program can help me in my research?
Most probably it can help you a lot if:
* You do some solid state calculations. Mostly DFT, but also MD or XRD analysis.
* You work with disordered materials: partial or/and mixed occupations structures.
* You have a very basic knowledge of CIF file structure and command line interface.

### What are the benefits of supercell software compare to any other solutions?
* All in one approach, instant start! You can work directly with CIF file within a few seconds.
* Powerful CLI with good verbosity.
* Electrostatic sampling method.
* Perfect performance.
* Integration with other software.
* A lot of useful examples in tutorial.
* Widely used by scientific community (more than 100 citations) in different materials.

### But supercell program can’t work with non-diagonal supercells, can it? Should I use another code for the task?
NO and NO. Supercell program can work with any supercells. Half of example supercell in the tutorial  have a conventional cell, thus such structures are non-diagonal supercells of a primitive cell. Unique internal algorithms calculates symmetry operations using universal math approach, which does not rely on spacegroup information. But you can’t create a non-diagonal supercell with the program CLI. This is a conscious choice to leave program as simple as possible. Are you ready to write down “primitive to fcc” transformation matrix just by memory? I am not. If you would like to use non-diagonal supercells with supercell, create it with, for example, VESTA GUI ([video guide](https://www.youtube.com/watch?v=Aw7goppiUHk)) or cif2cell CLI ([PDF](https://www-users.york.ac.uk/~mijp1/teaching/grad_FPMM/files/cif2cell.pdf)) and use it in the program.

### I need to calculate the output structures in DFT code (VASP, CASTEP, Wien2k etc), but supercell produce cif files only…?
Don’t worry! You can use excellent programs [(link)]() like cif2cell, OpenBabel or AiiDA to convert output cif files to any other structures. And you can use the result in VASP, ABINIT, CPMD, CRYSTAL, Quantum espresso, Elk etc

### What should I do, if supercell code is not working?
This is top one question. I wrote a special section with the same name in the [tutorial]().

### How can I help supercell project?
To be honest, nobody has ever asked me the question, but I would like to answer it so much, that I’ve decided to include it here. Now supercell is my hobby. Therefore, unfortunately, I don’t have much time to work with it. That’s why your help is very important for the project to stay alive. If you have anything valuable for other users, please share this. It can be, for example:
* well prepared bug report, of course.
* benchmark tests and performance suggestions.
* any input structures with description from your paper. I can put it to example folder.
* fair comparison with other similar programs. For example, share your story of switching to supercell from other program or vice versa.
* sharing your negative experience with supercell as well. It will help other users to avoid similar problems.
* anything else, that you think will be useful to share.
