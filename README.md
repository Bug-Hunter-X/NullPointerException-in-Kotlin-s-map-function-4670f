# Kotlin Map Function and Null Safety

This example demonstrates a common issue when using Kotlin's `map` function with lists that may contain null values.  Improper handling can lead to `NullPointerExceptions`. The code showcases how to safely handle nulls within the `map` operation to prevent such exceptions.

## The Problem

The `map` function transforms each element of a list.  However, if the list contains null values and you attempt to perform an operation directly on those nulls, a `NullPointerException` occurs. 

## The Solution

The solution involves using the safe call operator (`?.`) and the elvis operator (`?:`) to handle nulls gracefully.  The safe call operator checks for null before performing the operation, and the elvis operator provides a default value if the result is null.