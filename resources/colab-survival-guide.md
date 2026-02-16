# Colab Survival Guide (Quick)

Use this page when you get stuck in a notebook.

## 1) Run cells

- Run current cell: `Shift + Enter`
- Run without moving: `Ctrl + Enter`
- Run and insert new cell: `Alt + Enter`

## 2) Code cell vs Text cell

- **Code cell**: Python instructions (`print()`, variables, loops, imports)
- **Text cell**: Markdown notes, titles, reflections

Tip: if code appears as plain text, convert the cell type to **Code**.

## 3) Most common errors (and fixes)

### `NameError: name 'x' is not defined`

Meaning: variable/function not created yet.

Fix:
1. Run earlier cells first
2. Check spelling/capitalization
3. Re-run from top after runtime restart

### `ModuleNotFoundError`

Meaning: package not available in runtime.

Fix:
1. Install package in a cell (example):

```python
!pip install package-name
```

2. Re-run import cell

### Code worked before, now fails randomly

Meaning: runtime state is inconsistent.

Fix:
1. **Runtime → Restart runtime**
2. **Runtime → Run all**

## 4) Restart runtime safely

When in doubt:
1. Save notebook
2. Restart runtime
3. Run all cells from top to bottom

## 5) Save your work

- In Colab: **File → Save a copy in Drive**
- Optional local backup: **File → Download → Download .ipynb**

## 6) Fast troubleshooting checklist

If something is broken, do this in order:

1. Check you are in the right cell type (Code/Text)
2. Run cells from top to current one
3. Read the error line carefully (often points to exact problem)
4. Restart runtime + Run all
5. Ask a peer / teacher and show:
   - the error message
   - the cell that fails
   - what you already tried
