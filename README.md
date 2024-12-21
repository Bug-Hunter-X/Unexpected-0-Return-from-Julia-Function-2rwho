# Unexpected 0 Return from Julia Function

This repository demonstrates a common error in Julia where a function unexpectedly returns 0 for negative inputs due to a flaw in the conditional statement.

The `bug.jl` file contains the erroneous code, and `bugSolution.jl` provides the corrected version.

## Bug Description
The function `myfunction` is intended to square positive inputs and return 0 for non-positive inputs. However, it always returns 0 for any value less than or equal to 0, even if the intent was to perform a different calculation for negative inputs.

## Solution
The solution clarifies the conditional logic to handle negative numbers correctly. This was achieved by improving the conditions within the if-else block to return the correct result when `x` is negative.