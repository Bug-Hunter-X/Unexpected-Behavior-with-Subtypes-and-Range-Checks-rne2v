# Ada Subtype Range Check Bug

This example demonstrates a subtle bug related to how Ada handles subtype range checks.  The `if` condition does not detect the violation, as the range check is performed at assignment. 

The issue is described in the `bug.ada` file, and the solution is provided in `bugSolution.ada`. The solution uses the `in` operator to explicitly verify whether the variable is still within the subtype's range after the modification. 