# Silicon (2) - 2-bgw/4-absorption/converge_bands

There are four major convergence parameters in a Bethe-Salpeter equation
calculations, the number of:

1. Bands on the coarse grid
2. k-points on the coarse grid
3. Bands on the fine grid
4. k-points on the fine grid

The optical absorption spectrum of silicon is fairly easy to converge, so we
will instead study how the spectrum changes as we *worsen* some of the
convergence parameters. In this example, we will study how the spectrum is
affected by worsening convergence parameter (3).

Remember that, when you perform a calculation, you should check if all those 4
parameters are converged!


## Instructions

1. Run `./01-link_files.sh` to link the `WFN`, `bsemat.h5` and `epsmat.h5` files.

2. Edit `absorption.inp` and fill in the missing parameters.

3. Compare the `absorption.inp` file with your previous file. What's the
   difference?

4. Run `./02-run_absorption.run` to launch the absorption calculation.  While
   you wait: how do you expect your results to change as we decreased the
   number of bands?

5. Compare the `absorption_noeh.dat` file with the previous version, and
   `absorption_eh.dat` against the previous previous. What changed?  Is the
   calculation with one valence and one conduction band converged?
