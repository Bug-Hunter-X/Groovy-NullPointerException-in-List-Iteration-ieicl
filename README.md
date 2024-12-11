# Groovy NullPointerException in List Iteration

This example demonstrates a common error in Groovy when handling lists: a `NullPointerException` occurs when passing a `null` value to a method that iterates over a list.

The `bug.groovy` file contains the buggy code.  The `bugSolution.groovy` file provides the solution.

## Bug

The `myMethod` function iterates over a list of strings.  If a `null` list is passed, a `NullPointerException` will be thrown because the `each` method cannot operate on `null`.

## Solution

The solution is to add a null check before attempting to iterate over the list.