> [!note] Core Concept
> This chapter focuses on iterating through lists, generating numerical data, writing concise code with list comprehensions, slicing, and working with immutable lists (tuples).

## Looping Through a List
* **The `for` loop:** Executes the same block of code for every item in a list.
* **Syntax:** `for item in list_name:` followed by an indented block.
* **Indentation Rules:** Python strictly uses indentation to determine logical structure. Missing or unexpected spaces will trigger an `IndentationError`.
## Making Numerical Lists
* **`range()` Function:** Generates a sequence of numbers. `range(1, 5)` produces 1, 2, 3, and 4 (it stops *before* the second number).
* **`list()` Function:** Wraps `range()` to instantly create a list of numbers, e.g., `numbers = list(range(1, 6))`.
* **Simple Statistics:** Python has built-in functions for lists of numbers: `min(list)`, `max(list)`, and `sum(list)`.

## List Comprehensions
> [!tip] Efficiency
> A **list comprehension** combines a `for` loop and the creation of new elements into a single, highly readable line of code.
* **Syntax:** `squares = [value**2 for value in range(1, 11)]` generates a list of square numbers without needing an initialized empty list or an `.append()` method.

## Working with Part of a List (Slicing)
* **Creating a Slice:** Specify the start and stop indices separated by a colon, e.g., `players[0:3]`.
* **Omitted Indices:** Omitting the start index `[:3]` starts from the beginning. Omitting the stop index `[2:]` goes to the very end of the list.
* **Copying a List:** To make a true, independent copy of a list, use a full slice: `new_list = old_list[:]`. Simply setting `new_list = old_list` only copies the *reference*, meaning changes to one will affect the other.

## Tuples
> [!warning] Immutability
> A **tuple** is exactly like a list, except it is **immutable** (its values cannot be changed or modified once created).
* **Syntax:** Defined using parentheses instead of square brackets, e.g., `dimensions = (200, 50)`.
* **Redefining:** While you cannot modify an individual element inside a tuple (e.g., `dimensions[0] = 250` throws an error), you can overwrite the entire tuple variable with new values.