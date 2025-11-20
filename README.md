# Scamander
Counterfactual Explanations and How to Find Them

- *cf_eval* contains definition of the metrics used to evaluate the counterfactual explainers
- *experiments* contains the file to run to repeat the experiments
- *sace* contains the custom implementation of some counterfactual explainers

# Requirements
- Python > 3.7

## How to install required packages

### Linux / macOS

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

Adding Scamandar package directory to pythonpath so that we can import the experiments as is

```bash
cat >> .venv/bin/activate <<'BASH'
export PYTHONPATH="${PYTHONPATH:+${PYTHONPATH}:}$(cd "$(dirname "${BASH_SOURCE[0]}")/../.." && pwd)"
BASH
```
In case the venv is active, you have to run `deactivate` and `source .venv/bin/activate` again to take effect.

### Windows (PowerShell)

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install --upgrade pip
pip install -r requirements.txt
```