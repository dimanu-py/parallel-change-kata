# :rewind: Parallel Change Kata :rewind:

## Resources

These requirements and the initial state of the code are extracted from the original GitHub repository

[![Web](https://img.shields.io/badge/GitHub-unclejamal-14a1f0?style=for-the-badge&logo=github&logoColor=white&labelColor=101010)](https://github.com/unclejamal/parallel-change)

## What is parallel change?

Parallel change is a technique used in refactoring to make a series of incremental changes to a codebase without breaking the existing code.

It involves three steps:

1. **Expand**: Add new functionality to the codebase. It can be a class, method, variable...
2. **Migrate**: Move the existing code to the new functionality.
3. **Contract**: Remove the old code.

## Description

Modify the `ShoppingCart` class to handle multiple items instead of a single one.

We have the following rules:

1. Tests must be always green.
2. Use IDE refactor tools when possible.

## Objective

The main objective of the kata is to gain a deeper understanding of the parallel change technique and improve the ability to refactor
legacy code.
