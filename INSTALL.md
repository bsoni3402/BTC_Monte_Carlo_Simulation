# Installation Guide for VS Code

## Prerequisites

- [Python 3.9+](https://www.python.org/downloads/)
- [Visual Studio Code](https://code.visualstudio.com/)
- VS Code extensions: **Python** and **Jupyter** (by Microsoft)

## Setup Steps

### 1. Open the project in VS Code

```
code Monte_Carlo_Simulation
```

### 2. Create a virtual environment

Open the VS Code terminal (`Ctrl+`` ` or `Cmd+`` ` on Mac) and run:

```bash
python -m venv .venv
```

### 3. Activate the virtual environment

**Windows:**
```bash
.venv\Scripts\activate
```

**macOS / Linux:**
```bash
source .venv/bin/activate
```

### 4. Install the required libraries

```bash
pip install -r requirements.txt
```

This installs: `polars`, `pandas`, `numpy`, `matplotlib`, and `yfinance`.

### 5. Select the Python interpreter in VS Code

1. Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac)
2. Type **"Python: Select Interpreter"**
3. Choose the `.venv` interpreter (e.g., `./.venv/bin/python`)

### 6. Open and run a notebook

Open `BTC_monte_carlo.ipynb` or `AAPL_monte_carlo.ipynb` and click **Run All** to execute.

## Troubleshooting

- **"ModuleNotFoundError"**: Make sure the virtual environment is activated and you ran `pip install -r requirements.txt`.
- **Wrong kernel in Jupyter**: Click the kernel name in the top-right of the notebook and select the `.venv` Python interpreter.
