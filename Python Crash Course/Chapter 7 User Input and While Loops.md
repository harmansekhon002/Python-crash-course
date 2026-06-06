> [!note] Core Concept
> This chapter shifts programs from being static to interactive. You will learn how to accept input from the user using the `input()` function and how to keep programs running as long as certain conditions are true using `while` loops.

## 1. The `input()` Function
The `input()` function pauses the program and waits for the user to enter some text. Once the user presses Enter, the data is assigned to a variable.

* **String Default:** Everything entered via `input()` is interpreted as a string by Python, even if the user types a number.
* **Writing Clear Prompts:** Always tell the user exactly what you want them to do. If the prompt is long, assign it to a variable first and pass that variable to `input()`.

### Accepting Numerical Input
If you want to do math with user input, you must convert the string representation of the number into an actual integer using the `int()` function.

```python
age = input("How old are you? ")
age = int(age) # Converts the string "21" to the integer 21
```

> [!tip] The Modulo Operator (`%`)
> A useful tool when working with numerical input is the modulo operator (`%`). It divides one number by another and returns the **remainder**. It is frequently used to determine if a number is even or odd (e.g., `number % 2 == 0` means it is even).


## 2. Introducing `while` Loops
A `for` loop takes a collection of items and executes a block of code once for each item. A `while` loop runs as long as, or *while*, a certain condition remains `True`.

### Controlling the Loop
There are several ways to control how and when a `while` loop stops running.

| Technique | How It Works |
| :--- | :--- |
| **Conditional Test** | The loop runs while a simple comparison is `True` (e.g., `while current_number <= 5:`). |
| **Using a Flag** | A single boolean variable (e.g., `active = True`) dictates whether the entire program is active. The loop runs `while active:`. If any event happens that should stop the program, set `active = False`. |
| **The `break` Statement** | Immediately exits the loop entirely without running any remaining code in the loop, regardless of the conditional test. |
| **The `continue` Statement**| Skips the rest of the code inside the loop for the current iteration and jumps back to the top to evaluate the condition again. |

> [!warning] Infinite Loops
> Every `while` loop must have a way to stop running so it won't run forever. If your program gets stuck in an infinite loop, press `Ctrl + C` in the terminal to force it to quit.

## 3. Using `while` Loops with Lists and Dictionaries
You should not modify a list while iterating through it with a `for` loop, because Python will struggle to keep track of the items. To modify a list as you work through it, use a `while` loop.

### Common Use Cases
* **Moving Items:** Use a `while` loop with `.pop()` to pull items from an "unconfirmed" list, process them, and append them to a "confirmed" list until the first list is empty.
* **Removing Specific Values:** If a list contains multiple instances of a specific value (e.g., "cat"), a `while "cat" in pets:` loop combined with `pets.remove("cat")` will clear out all of them.
* **Filling a Dictionary:** Use a `while` loop alongside `input()` to prompt for both keys and values, storing them in an initially empty dictionary until the user decides to quit.