# Julia Floating-Point Precision Bug

This repository demonstrates an uncommon bug in Julia related to the handling of floating-point numbers close to zero within conditional statements.

The `bug.jl` file contains a function that squares positive inputs and returns 0 for non-positive inputs.  However, when given a floating-point number extremely close to zero, it unexpectedly returns 0 instead of a small positive value.

The `bugSolution.jl` file shows a corrected version that uses a tolerance to address the precision issue.

This bug highlights the importance of considering floating-point precision limitations when working with conditional logic in Julia.