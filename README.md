# Objective-C NSDecimalNumber Comparison Bug

This repository demonstrates a common error when comparing `NSDecimalNumber` objects in Objective-C. The problem arises from incorrectly interpreting the return value of the `compare:` method.

The `compare:` method returns an `NSComparisonResult` enum, which can be `NSOrderedAscending`, `NSOrderedSame`, or `NSOrderedDescending`.  Directly comparing this result with `YES` (1) or `NO` (0) can lead to incorrect logic and unexpected behavior.

The `bug.m` file shows the erroneous comparison. The `bugSolution.m` file demonstrates the correct way to handle this comparison.  Refer to the code for detailed examples.