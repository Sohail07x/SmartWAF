# SmartWAF Detection and Explainable AI — Module 1

## Module 1: Dataset Collection and Preparation

### Purpose
This module prepares the SmartWAF HTTP request dataset for the next ML module.

Pipeline:

Raw Excel Dataset
→ Dataset Loader
→ Dataset Inspection
→ YAML Schema Validation
→ Dataset Validation
→ Dataset Analysis
→ Master CSV Export
→ Automated Tests

## IMPORTANT: Dataset File

Place your exact dataset in:

data/raw/SmartWAF_Synthetic_Dataset_10000.xlsx

The program expects exactly that filename.

## VS Code Setup

Open the `SmartWAF_Module1_Complete` folder in VS Code.

Open Terminal:

```powershell
Ctrl + Shift + `
```

Create and activate the environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Install packages:

```powershell
python -m pip install -r requirements.txt
```

## Run Module 1

Run these commands from the project root:

```powershell
python -m src.data.inspect_dataset
python -m src.data.loader
python -m src.data.validate_dataset
python -m src.data.analyzer
python -m src.data.export_master
python -m pytest -q
```

## Expected Final Files

After successful execution:

- `reports/dataset_profile.json`
- `data/master/smartwaf_master_v1.csv`

## Expected Test Result

```text
6 passed
```
