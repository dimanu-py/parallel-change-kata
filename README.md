# :fast_forward: Parallel Change Kata :fast_forward:

[![Python](https://img.shields.io/badge/Python-3.11+-yellow?style=for-the-badge&logo=python&logoColor=white&labelColor=101010)](https://python.org)

## Resources

These requirements and the initial state of the code are extracted from the original GitHub repository

[![Web](https://img.shields.io/badge/GitHub-unclejamal-14a1f0?style=for-the-badge&logo=github&logoColor=white&labelColor=101010)](https://github.com/unclejamal/parallel-change)

## What is parallel change?

Parallel change is a technique used in refactoring to make a series of incremental changes to a codebase without breaking the existing code.

It involves three steps:

1. **Expand**: Add new functionality to the codebase. It can be a class, method, variable... Try to create new code instead of modifying existing implementations, also is a good idea to make new tests for this expanded code even if duplicates previous test behaviors.
2. **Migrate**: Move the existing code to the new functionality.
3. **Contract**: Remove the old code.

## Description

The kata contains two files:

1. `field`: the public interface of the code needs to stay as is, but the internal behavior of the class will change by adding a field class that will allow the `ShoppingCart` class to manage more than one item.
2. `method`: we want to introduce a new method in the `AuthenticationService` and deprecate the existing one without breaking the code in the process.

During the refactoring, we need to focus on:

1. Tests must be always green.
2. Use IDE refactor tools when possible.

> [!NOTE]
> The final state of the code after making both refactors are under two tags: one for the field scenario and the other for the method scenario.

## Objective

The main objective of the kata is to gain a deeper understanding of the parallel change technique and improve the ability to refactor
legacy code.

> [!IMPORTANT]
> We don't look for the code to be ultra-refactored creating new abstractions, design patterns, etc. Remember, we want to practice the parallel change process.

## Configuration

The project can be configured either by using `pip` or `pipenv`. Both ways will be explained.

<details><summary>Using pip</summary>

1. Create a virtual environment:
    ```bash
    python -m venv .venv
    ```
2. Activate the virtual environment:
    ```bash
    source .venv/bin/activate # Linux / Mac
    .venv\Scripts\activate # Windows
    ```
3. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```
</details>

<details><summary>Using pipenv</summary>

1. Install pipenv:
    ```bash
    pip install pipenv
    ```
2. Create a virtual environment with desire python version
    ```bash
    pipenv --python 3.11
    ```
   
    By default it will create the virtual environment outside the project. To create it inside the project, use the following command:
    ```bash
    PIPENV_VENV_IN_PROJECT=1 pipenv --python 3.11
    ```
3. Install the dependencies:
    ```bash
    pipenv install
    ```
</details>

## Running the tests

To run the tests, execute one of the following commands:

```bash
pytest
```

or

```bash
pipenv run test
```

### Visit my GitHub profile to see all solved katas 🚀

[![Web](https://img.shields.io/badge/GitHub-Dimanu.py-14a1f0?style=for-the-badge&logo=github&logoColor=white&labelColor=101010)](https://github.com/dimanu-py/code-katas)
