How to differentiate collective variables in free energy codes
=============================

[Toni Giorgino](https://www.giorginolab.it)

This code accompanies [my talk](plumed2019_autodiff_web.pdf)
at CECAM's [Open source software for enhanced-sampling simulations](https://www.cecam.org/workshop1749/),
taking place on 25-27 July 2019 at Università della Svizzera Italiana,
Lugano.

The subdirectories reproduce and simplify the code provided  with
the following paper:

> T. Giorgino, How to differentiate collective variables in free energy codes: Computer-algebra code generation and automatic differentiation, Computer Physics Communications 228, 258–263 (2018) [doi](http://dx.doi.org/10.1016/j.cpc.2018.02.017) [arxiv](https://arxiv.org/abs/1709.06780) [plumID:19.011](https://www.plumed-nest.org/eggs/19/011/)

In particular you will find

* [stan-math-examples](stan-math-examples), which demonstrates the use of the Stan Math library (outside PLUMED)
* [symbolic-code-generation-examples](symbolic-code-generation-examples), which shows how to use SymPy to automatically generate code (outside PLUMED)

To see how the two approaches can be integrated in PLUMED CVs, including help and regression tests, see the original [plumed2-automatic-gradients](https://github.com/tonigi/plumed2-automatic-gradients) repository, and in particular:

* [src/curvature_codegen](https://github.com/tonigi/plumed2-automatic-gradients/tree/automatic-gradient-computation/src/curvature_codegen), with regtests in  [regtest/curvature_codegen](https://github.com/tonigi/plumed2-automatic-gradients/tree/automatic-gradient-computation/regtest/curvature_codegen) 
* [src/curvature_autodiff](https://github.com/tonigi/plumed2-automatic-gradients/tree/automatic-gradient-computation/src/curvature_autodiff), with regtests in 
[regtest/curvature_autodiff](https://github.com/tonigi/plumed2-automatic-gradients/tree/automatic-gradient-computation/regtest/curvature_autodiff)




