# Silicon (2) - 2-bgw/4-absorption/converge_kpts

There are four major convergence parameters in a Bethe-Salpeter equation
calculations, the number of:

1. Bands on the coarse grid
2. k-points on the coarse grid
3. Bands on the fine grid
4. k-points on the fine grid

In this example, we will study how the spectrum is affected by worsening
convergence parameter (4).

Remember that, when you perform a calculation, you should check if all 4
parameters are converged!


## Instructions

1. Go to subdirectories `wfn_fi/` and `wfnq_fi/` to generate new fine-grid wave
   function files. Follow the instructions in the corresponding `README.md`
   files.

2. Run `./01-link_files.sh` to link the `WFN`, `bsemat.h5` and `epsmat.h5`
   files.

3. Edit `absorption.inp` and fill in the missing parameters.

4. Run `./02-run_absorption.run` to launch the absorption calculation.  While
   you wait: how do you expect your results to change as we decreased the
   number of k-points? How do the previous and the new k-point sampling
   compare?

5. Compare the `absorption_noeh.dat` file with the previous version, and
   `absorption_eh.dat` against the previous previous. What changed? Is this new
   calculation converged with respect to k-point sampling?
