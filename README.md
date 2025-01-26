# ugp-pinn
 Modelling a two-level atom’s saturated absorption spectra using a Physics Informed Neural Network (PINN)


# TODO:
1. figure out how to formulate the problem exactly for an PINN
2. basic two-level atom qutip model: find refractive index etc.
3. lorentz model creation PINN

## Project Pipeline
1. For training data, break the given material down into a standard format to express its nuclear geometry (coulomb-matrix)? This is an open question - every paper I have seen dedicates a section to methodology to deriving which m
2. Find the excitement energies using Monte-carlo or molecular dynamics simulators: this has been demonstrated to be learnt by ML for certain classes of materials. 
3. Calculate the **basic** spectra linewidth etc., and then add effects like Doppler broadening
4. Compute transition intensities (do not know how to approach yet).
5. Compute line-splitting/field effects.
6. Port this data to the ML model 
    a. Less sample requirements
    b. Robust predictions via physics informed (PI)regularizer
    c. Basically curve-fitting?



## Questions
1. Do we want to predict the linewidths too? All this depends on the type of training data we are aiming for.
2. The role of DFT?