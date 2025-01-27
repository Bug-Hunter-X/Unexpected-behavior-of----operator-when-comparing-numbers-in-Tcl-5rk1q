# Tcl Bug: Unexpected == behavior with numbers
This repository demonstrates a common error in Tcl when comparing numbers using the `==` operator. The `==` operator in Tcl performs string comparisons, which can lead to unexpected results when comparing numbers that are stored as strings.

## Bug Description
The provided Tcl procedure `buggyProc` attempts to compare two numerical inputs. However, because it uses the `==` operator, it will only work correctly if inputs are numeric. If inputs are strings, the result will be unexpected. 

## Solution
The solution is to use the `expr` command for numerical comparisons to ensure that the numbers are compared numerically instead of as strings.  

## How to reproduce
1. Run `bug.tcl`
2. Observe the incorrect result. 
3. Run `bugSolution.tcl`
4. Observe the corrected result.