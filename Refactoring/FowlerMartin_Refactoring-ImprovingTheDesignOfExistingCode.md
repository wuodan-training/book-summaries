---
title: "Refactoring: Improving the Design of Existing Code"
---

**Author: Martin Fowler | Publisher: Addison-Wesley | Summary: Stefan Kuhn**

# Chapter 1: Refactoring: A First Example

>When you have to add a feature to a program but the code is not structured in a convenient way, first refactor the program to make it easy to add the feature, then add the feature.

## The First Step in Refactoring

>Before you start refactoring, make sure you have a solid suite of tests. These tests must be self-checking.

## Decomposing the ‘statement’ Function

Try to identify points that separate different parts of the overall behavior.

Example: Long function with a large switch statement in the middle.

Extract function:

1. Extract the large switch statement to a function.

1. Give the function a meaningful name in camelcase

1. Check for variables that will no longer be in scope.

1. Compile and run tests immediately after each small change

1. Commit the change to local version version control system

Essence of the refactoring process: small changes and testing after each
change. Commit after each successful refactoring, so I can easily get back to a working state. Squash changes into more significant commits before I push the changes to a shared repository

*Extract Function* should be supported by the IDE:
IntelliJ keyboard shortcuts:
- 