# VHDL Counter with Incorrect Sensitivity List

This repository demonstrates a common error in VHDL: an incorrect sensitivity list in a concurrent signal assignment.

The `bug.vhdl` file contains a VHDL counter that uses a concurrent signal assignment (`count <= internal_count;`) without a sensitivity list. This means that the `count` signal is not updated whenever `internal_count` changes.  The result will be that the output `count` will not update correctly. 

The `bugSolution.vhdl` file provides a corrected version of the counter with a proper sensitivity list, ensuring that the output accurately reflects the internal count.

This example highlights the importance of correctly specifying sensitivity lists in VHDL to avoid unexpected behavior and ensure proper signal updates.