# VHDL Counter Overflow Bug

This repository demonstrates a common bug in VHDL code: an integer overflow in a counter.  The `buggy_counter.vhdl` file contains the buggy code, which fails to properly handle the upper bound of the counter, leading to unpredictable behavior. The `fixed_counter.vhdl` demonstrates a corrected implementation.

## Bug Description
The original VHDL counter implementation does not reset the counter correctly when it reaches its maximum value (15). This can result in an integer overflow and unexpected behavior. 

## Bug Solution
The solution involves ensuring proper handling of the counter's upper bound. When the counter reaches 15, it is reset to 0.  The solution is implemented in `fixed_counter.vhdl`.