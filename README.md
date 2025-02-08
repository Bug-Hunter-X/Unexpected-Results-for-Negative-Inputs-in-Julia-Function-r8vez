# Julia Function Bug: Unexpected Negative Input Handling

This repository demonstrates a common bug in Julia functions: unexpected results for negative inputs due to incorrect handling of the negative sign in the `else` block. The original function fails to correctly square negative numbers, leading to inaccurate outputs. The solution provides a corrected version that addresses this issue.

## Bug Description

The `myfunction` in `bug.jl` intends to return the square of the input number, handling negative numbers correctly. However, the `else` block incorrectly calculates `-x^2`, which gives an incorrect result for negative inputs. The function produces incorrect results for negative numbers. 

## Solution

The `bugSolution.jl` file contains the corrected function. It addresses the issue by correctly calculating the square of the input, regardless of its sign. This ensures that the function produces correct outputs for all input values. The corrected function explicitly squares the input number using `abs(x)^2`. 