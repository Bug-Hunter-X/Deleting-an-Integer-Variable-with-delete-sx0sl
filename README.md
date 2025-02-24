# Deleting an Integer Variable with delete
This repository demonstrates a common C++ error: attempting to use the `delete` operator on a non-dynamically allocated variable.  The `bug.cpp` file contains the erroneous code, while `bugSolution.cpp` provides a corrected version.

## The Problem
The `delete` operator is used to release memory that was previously allocated using `new`. Attempting to use `delete` on a variable that was not allocated with `new` (like a stack-allocated variable) leads to undefined behavior, possibly causing crashes or data corruption.

## The Solution
The corrected code removes the erroneous `delete` statement.  Stack-allocated variables are automatically managed by the compiler and do not require manual deallocation.
