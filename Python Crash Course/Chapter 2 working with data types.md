## Variables
Variables are labels that you assign to values. They are not "boxes" that hold data, but rather references to the data.

```python
message = "Hello Python world!"
print(message)
```

**Naming Rules & Best Practices:**
- Must contain only letters, numbers, and underscores.
- **Cannot** start with a number.
- **Cannot** contain spaces (use underscores `_` instead, e.g., `user_name`).
- Avoid Python keywords and built-in function names (like `print`).
- Keep names descriptive, concise, and use lowercase letters.

---

## Strings
A string is a series of characters enclosed in either single (`'`) or double (`"`) quotes. This flexibility allows you to easily include quotes or apostrophes within your text.

### Manipulating Case
Python has built-in methods to change the case of strings:
```python
name = "ada lovelace"
print(name.title()) # Output: Ada Lovelace
print(name.upper()) # Output: ADA LOVELACE
print(name.lower()) # Output: ada lovelace
```

### F-Strings (Formatted String Literals)
A powerful way to insert variable values directly into a string. Place an `f` before the opening quote and enclose variables in `{}`.
```python
first_name = "ada"
last_name = "lovelace"
full_name = f"{first_name} {last_name}"
```

### Whitespace & Stripping
You can format text using non-printing characters, and clean up accidental whitespace using strip methods.
- **Tabs & Newlines:** `\t` (tab), `\n` (newline).
- **Stripping Space:**
  - `rstrip()`: Removes right-side whitespace.
  - `lstrip()`: Removes left-side whitespace.
  - `strip()`: Removes whitespace from both sides.

```python
favorite_language = 'python '
favorite_language = favorite_language.rstrip() # Permanently removes the space
```

## Numbers

### Integers and Floats
- **Integers:** Whole numbers. You can add (`+`), subtract (`-`), multiply (`*`), divide (`/`), and find exponents (`**`).
- **Floats:** Any number with a decimal point. (Note: floating-point math can sometimes result in arbitrary decimal places due to how computers represent numbers).

### Syntactic Sugar & Readability
```python
# Grouping large numbers with underscores (Python ignores the underscores)
universe_age = 14_000_000_000

# Multiple assignment in a single line
x, y, z = 1, 2, 3
```

> [!important] Constants in Python
> Python doesn't have a built-in constant type. By convention, write the variable name in **ALL_CAPS** to indicate to other programmers that the value should never be changed.
> ```python
> MAX_CONNECTIONS = 5000
> ```

## Comments
Comments allow you to write notes in English within your programs. Python ignores them when running the code. Use them to explain the *why* behind your logic.

```python
# Say hello to everyone.
print("Hello Python people!")
```

## The Zen of Python
A brief set of guiding principles for writing good Python code, written by Tim Peters. 

> [!quote] 
> You can view this easter egg in your terminal or IDE by running:
> ```python
> import this
> ```
> *Key takeaways:*
> - Simple is better than complex.
> - Readability counts.
> - There should be one—and preferably only one—obvious way to do it.