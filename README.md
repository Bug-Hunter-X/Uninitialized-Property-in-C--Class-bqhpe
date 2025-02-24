# Uninitialized Property in C# Class

This example demonstrates a common issue in C# where a class property is not explicitly initialized in the constructor.  This can lead to unexpected default values (0 for numeric types, null for reference types) and potential runtime errors.

The `bug.cs` file shows the problem: `MyProperty` is not initialized, leading to unpredictable behavior if it's accessed before being assigned a value.

The `bugSolution.cs` file shows a corrected version:  `MyProperty` is explicitly initialized in the constructor, ensuring predictable behavior.