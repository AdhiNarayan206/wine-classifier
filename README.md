# Projects

1. Wine quality analysis with feature importance

Walkthrough: [solid_projects.ipynb](solid_projects.ipynb)

## Setup

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

## Wine Analysis

Located in `wine_agent/` with `wine_quality.csv`.

Files:
- [wine_agent/data.py](wine_agent/data.py)
- [wine_agent/model.py](wine_agent/model.py)
- [wine_agent/train.py](wine_agent/train.py)
- [wine_agent/agent.py](wine_agent/agent.py)

Run:
```powershell
# Train model
.\venv\Scripts\python.exe -m wine_agent.train

# Ask analytical questions
.\venv\Scripts\python.exe -m wine_agent.agent --question "What chemical factors most strongly predict high-quality wine?"
```

Outputs:
- `wine_agent/outputs/wine_training_metrics.csv`
- `wine_agent/outputs/wine_test_metrics.csv`
- `wine_agent/outputs/wine_feature_importance.csv`
- `wine_agent/outputs/wine_test_predictions.csv`
- `wine_agent/outputs/wine_classifier.pth`

