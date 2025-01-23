# Python: Handling ZeroDivisionError in Average Calculation

This repository demonstrates a subtle case of a `ZeroDivisionError` that can occur when calculating the average of a list of numbers in Python. The code includes explicit handling for an empty list, but fails gracefully when the list contains only zeros.

The `bug.py` file contains the flawed code. The `bugSolution.py` demonstrates a corrected version that addresses the issue.

The issue is subtle because the explicit `if not numbers` check only addresses the empty list scenario. A list containing all zeros still leads to division by zero although the sum will be zero which usually evaluates to false in an if conditional statement. 

This example highlights the importance of robust error handling, especially when dealing with numerical operations.