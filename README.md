<div align="center">

# Slot Generator

**A Jupyter/Google Colab workflow for generating slot-game reel tables and symbol-ratio spreadsheets from CSV input data.**

</div>

## Quick Start

The project is notebook-driven. Open [`slot_generate.ipynb`](slot_generate.ipynb) locally or run it in Google Colab:

[Open `slot_generate.ipynb` in Google Colab](https://colab.research.google.com/github/iinoshirozheng/Slot_Generator/blob/main/slot_generate.ipynb)

For a local Jupyter environment, the notebook currently imports NumPy and pandas:

```bash
pip install jupyter numpy pandas
jupyter notebook slot_generate.ipynb
```

## Input

CSV inputs are read from the repository's `data/` directory by default:

```python
dir_path = "data"
```

When running in Colab, upload the input CSV files into the notebook session's `data` directory before executing the generation cells. The notebook also contains adjustable symbol labels and generation parameters; review those cells for the target game configuration before running it on production data.

## Output

The current repository includes examples of the notebook's generated spreadsheet outputs, including:

- `Symbol比例_NORMAL_*.xlsx`
- `Symbol比例_FREE_*.xlsx`
- `生成的輪帶表_NORMAL_*.xlsx`
- `生成的輪帶表_FREE_*.xlsx`

These are generated artifacts/examples, not hard-coded performance guarantees or universal slot configurations.

## Repository Layout

```text
slot_generate.ipynb   primary generation workflow
data/                  CSV input data
*.xlsx                 generated/example reel and symbol-ratio outputs
```

Older notebooks that existed earlier in the repository history are no longer part of `main`; `slot_generate.ipynb` is the current primary workflow.

## Project Status

This is a notebook-oriented utility rather than a packaged CLI/library. The notebook itself is the source of truth for current labels, parameters, and generation logic.
