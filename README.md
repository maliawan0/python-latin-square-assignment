# Latin Square Validator — Python Assignment

First programming assignment (2022). Python routines that validate whether a matrix forms a **Latin square** — no value repeated within any row or any column.

## The problem

Given a 2D list, return `True` only if:

- every element is numeric (any string invalidates the matrix), and
- no two adjacent-or-equal values repeat along a row, and
- no value repeats down a column

The implementation in [`L21-5648.ipynb`](L21-5648.ipynb) walks the matrix twice — once row-major to check horizontal constraints, once column-major for vertical ones — returning early on the first violation.

## Example

```python
test1 = [[1, 2, 3],
         [2, 3, 1],
         [3, 1, 2]]     # True  — valid Latin square

test2 = [[1, 2, 3, 4],
         ...]           # False — repeats found
```

## Running it

```bash
jupyter notebook L21-5648.ipynb
```

Pure Python — no dependencies beyond Jupyter.

## Scope

Earliest work in this account, kept as a record of where the coursework started.
