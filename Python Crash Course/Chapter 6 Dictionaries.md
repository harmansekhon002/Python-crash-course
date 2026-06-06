
> [!note] Definition
> A **dictionary** is a collection of **key-value pairs**. Each key is connected to a value, and you use the key to access its associated value. They are wrapped in curly braces `{}`.


## Basic Operations
* **Create:** `alien = {'color': 'green', 'points': 5}`
* **Access (Bracket):** Use the key inside square brackets: `print(alien['color'])`
* **Access (`.get()`):** Safely retrieves a value without causing a `KeyError` if the key doesn't exist: `alien.get('points', 'No points assigned')`
* **Add/Modify:** Assign a value to a new or existing key: `alien['x_position'] = 25`
* **Remove:** Permanently delete a key-value pair using `del`: `del alien['points']`

## Looping Through a Dictionary
Python provides specific methods depending on what part of the dictionary you want to iterate over.

| Method | Purpose | Syntax Example |
| :--- | :--- | :--- |
| **`.items()`** | Access both keys and values. | `for key, value in alien.items():` |
| **`.keys()`** | Access only the keys (this is also the default). | `for key in alien.keys():` |
| **`.values()`** | Access only the values. | `for value in alien.values():` |

> [!tip] Organizing Loop Output
> * **Sort:** Wrap the method in `sorted()` to loop alphabetically, e.g., `for name in sorted(users.keys()):`.
> * **Remove Duplicates:** Wrap `.values()` in `set()` to loop through only unique values, e.g., `for language in set(languages.values()):`.

## Nesting
Nesting allows you to store complex data structures inside one another.
* **List of Dictionaries:** Storing multiple dictionaries inside a single list (e.g., a list of many different alien dictionaries).
* **List in a Dictionary:** Storing a list as a value for a specific key (e.g., `pizza = {'crust': 'thick', 'toppings': ['mushrooms', 'cheese']}`).
* **Dictionary in a Dictionary:** Storing a dictionary as the value for another dictionary's key (e.g., a dictionary of users, where each user's value is a nested dictionary of their profile details).