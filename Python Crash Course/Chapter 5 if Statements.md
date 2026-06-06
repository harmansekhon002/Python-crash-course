> [!note] Core Concept
> This chapter focuses on controlling program flow using **conditional tests** and **`if` statements** to execute code only when specific conditions are met.

## Conditional Tests
At the heart of every `if` statement is an expression that evaluates to either `True` or `False` (a boolean value).

* **Equality:** `==` checks if values are exactly equal (case-sensitive).
* **Inequality:** `!=` checks if values are not equal.
* **Numerical Comparisons:** `<`, `>`, `<=`, `>=`.
* **Multiple Conditions:** * `and`: Both conditions must be `True`.
  * `or`: At least one condition must be `True`.
* **List Membership:**
  * `in`: Checks if a specific value exists inside a list.
  * `not in`: Checks if a value is absent from a list.

## Types of `if` Statements
Python processes `if` statements from top to bottom and executes the indented block of the first `True` condition it encounters.

| Structure | Use Case |
| :--- | :--- |
| **`if`** | A simple test. If `True`, the code runs. If `False`, nothing happens. |
| **`if-else`** | Provides a specific alternative block of code to run when the `if` test fails. |
| **`if-elif-else`** | Used for testing more than two possible situations. The `else` block is optional and acts as a final catch-all. |

> [!warning] The `elif` Chain Limit
> An `if-elif-else` block stops evaluating as soon as it finds one test that passes. If you need to check whether *multiple* conditions are true simultaneously, use a series of independent simple `if` statements instead.

## Using `if` Statements with Lists
* **Checking for Special Items:** Combine a `for` loop with an `if` statement to apply different behaviors to specific items as you iterate.
* **Checking if a List is Empty:** In Python, the name of a list evaluates to `True` if it contains at least one item, and `False` if it is completely empty.
  ```python
  cars = []
  if cars:
      print("List is not empty.")
  else:
      print("List is empty.")
  ```