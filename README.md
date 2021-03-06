# Induction Equation


[![License](https://licensebuttons.net/l/by-nc-nd/3.0/88x31.png)](https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1434408.svg)](https://doi.org/10.5281/zenodo.1434408)


This is a set of tools for numerically solving the
[nonlinear magnetic induction equation](https://github.com/MuMPlaCL/InductionEq/blob/master/docs/induction_equation.ipynb)
with OpenCL. It is intended as a research tool to investigate different properties of the linear and nonlinear induction equation
for user specified testcases. All numerical aspects are encapsulated in OpenCL kernels. The OpenCL host side is abstracted
with the help of [MatCL](https://github.com/MuMPlaCL/MatCL), an OpenCL interface for MathWorks Matlab. This provides
the user with an intuitive and easy way of handling and processing input and output data without any intricate knowledge of
OpenCL and allows for interactive development. Support for [Julia](https://julialang.org/) is currently under development
and will be provided in the near future. Usage of the OpenCL kernels is not limited to Matlab or Julia; on the contrary
they can be used with any kind of host code or application that supports OpenCL.

This project is the base of current mathematical and physics research. Hence, special emphasis is placed on the computational
mathematics, meaning the form of discretization, methods of different order for spatial discretization and time integration
and admissable boundary conditions for the linear and nonlinear induction equation. First results have been published on
[arXiv.org](https://arxiv.org/abs/1810.01397).

Exemplary testcases for the linear and nonlinear induction equation can be found in the `examples` folder.
Specific readme files are available in the subfolders and additional comments are provided in the source files.

This is still very much work in progress. If you have any questions or want to contribute feel free to contact us.

## Prerequisites & Setup

To run the examples the following must be installed:

 - OpenCL Driver (CPU or GPU)
 - OpenCL C++ Headers (e.g. provided by the OpenCL vendors SDKs)
 - Mathworks Matlab
 - [MatCL](https://github.com/MuMPlaCL/MatCL)

 For ease of use you can add `MatCL` to the search path of Matlab.


## Citation

This software can be cited as:
```
@misc{ranocha2018induction,
  title={{InductionEq}. {A} set of tools for numerically solving the nonlinear
         magnetic induction equation with {H}all effect in {OpenCL}.},
  author={Ranocha, Hendrik and Ostaszewski, Katharina and Heinisch, Philip},
  month={09},
  year={2018},
  howpublished={\url{https://github.com/MuMPlaCL/InductionEq}},
  doi={10.5281/zenodo.1434408}
}
```
The accompagnying article describing the spatial discretizations in detail is:
```
@online{ranocha2018numerical,
  title={Numerical Methods for the Magnetic Induction Equation with Hall Effect
         and Projections onto Divergence-Free Vector Fields},
  author={Ranocha, Hendrik and Ostaszewski, Katharina and Heinisch, Philip},
  year={2018},
  month={10},
  note={Submitted},
  eprint={1810.01397},
  eprinttype={arxiv},
  eprintclass={math.NA}
}
```


 ## License

This project is licensed under the terms of the Creative Commons [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/legalcode) license.


 ## Disclaimer

Product and company names may be trademarks or registered trademarks of their respective holders.
Use of them does not imply any affiliation with or endorsement by them or their affiliates.
Everything is provided as is and without warranty. Use at your own risk!
