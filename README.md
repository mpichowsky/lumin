# lumin


## Features
-- none

---

## Getting Started

### 1) Clone the repository
```bash
  # Using HTTPS
  git clone https://github.com/mpichowsky/lumin.git
  cd lumin
  # Or using SSH
  git clone git@github.com:mpichowsky/lumin.git
  cd lumin
``` 
### 2) Create a local Python environment
Recommended: Python 3.10+

Option A — Bash / Command line (cross-platform with venv)
```bash
# From the repo root
python -m venv .venv    # or: python3 -m venv .venv
# Activate the environment
# macOS / Linux:
source .venv/bin/activate
# Windows (PowerShell):
.venv\Scripts\Activate.ps1
# Windows (cmd):
.venv\Scripts\activate.bat

# Upgrade pip (recommended)
python -m pip install --upgrade pip
```

Option B — VS Code: “Python: Create Environment”
Open this folder in VS Code.

Open the Command Palette (View → Command Palette… or Ctrl+Shift+P / Cmd+Shift+P).

Run Python: Create Environment.

Choose Venv (or Conda if you prefer).

Select a Python interpreter (e.g., Python 3.10+).

If prompted, allow VS Code to install dependencies from requirements.txt.

If not prompted, you can still install them manually (see next step).

VS Code will create .venv (or a conda env) and set it as the workspace interpreter.
You can confirm in the status bar (bottom-right) or with Python: Select Interpreter.

3) Activate the environment & install dependencies
If you created the env with VS Code and it auto-installed dependencies, you can skip to “Run a quick check.” Otherwise:

```bash
# Install dependencies
pip install -r requirements.txt
```

4) Run a quick check
```bash
python -c "import sys; print('Python', sys.version); print('Env OK')"
```
If the command runs without errors, you’re good to go.

### 3) Adding new dependencies
```bash
pip install <package>
pip freeze > requirements.txt   # update lock for collaborators/CI
```

