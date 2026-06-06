> [!note] Definition
> A **list** is an ordered collection of items inside square brackets, e.g., `bicycles = ['trek', 'redline']`.

## Accessing Elements
* **Zero-based indexing:** `bicycles[0]` accesses the first item.
* **Negative indexing:** `bicycles[-1]` safely accesses the last item.

## Modifying & Adding
* **Modify:** Reassign directly via `bicycles[0] = 'new'`.
* **Append:** `.append('val')` adds to the end.
* **Insert:** `.insert(0, 'val')` adds at a specific index.

## Removing Elements
* **Delete:** `del bicycles[0]` permanently removes by index.
* **Pop:** `.pop()` removes and returns the last item (or specific index).
* **Remove:** `.remove('val')` deletes the *first* occurrence of a specific value.

## Organizing Lists
* **Permanent Sort:** `.sort()` orders alphabetically (`reverse=True` for descending).
* **Temporary Sort:** `sorted(list_name)` returns a sorted copy.
* **Reverse Order:** `.reverse()` flips the current order permanently.
* **Length:** `len(list_name)` returns the total item count.

> [!warning] IndexError
> Asking for an index that doesn't exist causes an `IndexError`. Always use `-1` to safely grab the final element of a list of unknown length.

