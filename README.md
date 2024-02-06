Author:
Shi Chung
Github link:
https://github.com/josephshichung?tab=repositories

Summary:
In this assignment, I received an existing implementation of the classifyTriangle program (in Triangle.py) and a starter test program (TestTriangle.py). The objective was to develop a set of tests for the existing program, identify and fix defects, and report the testing results. Below is a detailed report of the process and outcomes.

Honor Pledge:
I affirm that the work submitted for this assignment is my own and adheres to the principles of academic integrity.

Part 1: Initial Test Results
Test set:
Test ID	Input	Expected Results	Actual Result	Pass/Fail
1	3,4,5	Right Triangle	NotATriangle	Fail
2	1,1,1	Equilateral	Equilateral	Pass
3	5,5,4	Isoceles	                 	Isoceles  	Pass
Detailed Results:

Test 1 (3, 4, 5):
The program incorrectly identified a right-angled triangle as "NotATriangle." This defect was identified during the initial tests.

Test 3 (5, 5, 4):
The program correctly identified an isosceles triangle. This case helped validate the program's ability to handle isosceles triangles.

...


Summary Results:
Tests Planned: 3
Tests Executed: 3
Tests Passed: 2
Defects Found: 1

Part 2: Improved classifyTriangle Logic
Source Code:
Triangle.py
Test Set:
Text ID	Input	Expected Results	Actual Result	Pass/Fail
1	3,4,5	Right Triangle	Right Triangle	Pass
2	1,1,1	Equilateral	Equilateral	Pass
3	5,5,4	Isosceles	Isosceles	Pass

Summary Results:
Tests Planned: 3
Tests Executed: 3
Tests Passed: 3
Defects Found: 0
Defects Fixed: 1

Improvements in Part 2:
The defects identified during the initial tests were addressed by refining the logic in the `classifyTriangle` function. Specifically, the right-angled triangle case (Test 1) was corrected, ensuring accurate triangle classification.

Challenges:
Navigating through the existing code and understanding its intricacies presented some challenges. However, this process contributed to a deeper understanding of the importance of thorough testing.

Conclusion:
This assignment provided a practical experience of testing and improving an existing program. It emphasized the importance of thorough testing and iterative development to identify and fix defects. The GitHub repository containing the code for this assignment is named Triangle567.
Test Run	Tests Planned	Test Executed	Tests Passed	Defects Found	Defects Fixed
1	9	7	5	2	0
2	9	9	9	0	2


Strategy for Test Case Sufficiency:
The approach to determining test case sufficiency involved comprehensive coverage across various scenarios. The criteria for sufficiency were as follows:
Triangle Type Variation:
Ensuring test cases cover different triangle types, including equilateral, isosceles, and scalene.
Incorporating scenarios involving right-angled triangles.
Boundary and Edge Cases:
Testing with both small and large values to address potential boundary concerns.
Examining cases where the sum of two sides equals the third side.
Handling Invalid Inputs:
Verifying the program's response to invalid inputs, such as negative values or non-numeric entries.
Factor Combination:
Creating test cases that combine multiple factors, like a right-angled isosceles triangle.
Exploring Defect Scenarios:
Constructing tests intentionally triggering defects identified in initial testing.
Confirming defect resolution through subsequent testing.
Iterative Approach:
Iteratively running test cycles, integrating feedback to enhance the test suite.
Continuously updating and expanding the test suite with new scenarios and edge cases.

The objective was to strike a balance between comprehensive coverage and practicality, ensuring the test suite effectively identifies defects while remaining manageable and sustainable. Each test run contributed to refining the test suite and enhancing the overall quality of the classifyTriangle function.

This strategy aimed to instill confidence in the correctness and robustness of the program across diverse input scenarios.

Reflection:
Reflecting on this assignment, I learned the significance of comprehensive testing and the iterative process of software development. The initial defects in the program were successfully identified, addressed, and verified through an improved set of test cases.

