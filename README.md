# STV-TV

## Overview

This repository contains the work for the STV-TV project. It holds three task folders (Task 1, Task 2, Task 3) with analysis notebooks and reports, plus a final presentation PDF. The README below documents every file and gives guidance on how to open and reproduce the work.

## Repository structure (top-level)

./
- `.git/` - git metadata (repo root)
- `README.md` - this file
- `STC_TV - Final Presentation.pdf` - final presentation covering the project (see "Final presentation" section)
- `Task 1/` - exploratory data analysis
- `Task 2/` - prediction / time-series experiments
- `Task 3/` - recommendation system experiments

> Note: macOS system file `.DS_Store` may be present; it is not part of the project.

## Files & folders — detailed description

### STC_TV - Final Presentation.pdf

- Location: repository root
- What it is: The final presentation summarizing the project results, conclusions and recommendations. Use any PDF viewer to open it.

### Task 1/

Files:
- `Task 1 - Report - STC_T1.pdf`
	- A formal report describing Task 1 objectives, methods, findings and recommendations. Open with a PDF viewer.

- `Task 1 - STC_T1 - Exploratory Data Analysis.ipynb`
	- A Jupyter Notebook performing exploratory data analysis (EDA) on the Task 1 dataset(s). This notebook likely contains data loading, cleaning, visualization and preliminary observations. To run or view:
		- Locally: use Jupyter Notebook / Jupyter Lab (python environment with needed packages like pandas, matplotlib, seaborn). Open the `.ipynb` file in Jupyter.
		- In the cloud: upload to Google Colab (File → Upload notebook) or use nbviewer to inspect static output.

Recommended order: read the EDA notebook first to follow the exploratory steps, then read the report for conclusions.

### Task 2/

Files:
- `Task 2 - Prediction - Report.pdf`
	- The written report for Task 2 describing the prediction approach, experiments, metrics and conclusions.

- `Task 2 - STC_T2 - TimeSeries_ARIMA_Hozaifa.ipynb`
	- A Jupyter Notebook focused on time-series forecasting using ARIMA (or related) models. Contains code, plots, and results for the forecast experiments.

- `Task 2 - STC_T2_Predictions.txt`
	- Text file containing the model's predictions (likely one prediction per line or CSV-like). Use a text editor or load with pandas (`pd.read_csv('Task 2 - STC_T2_Predictions.txt', header=None)`) to inspect.

- `Task 2 - STC_TV_Dataset_T2.xlsb`
	- The Task 2 dataset in Excel binary format (.xlsb). This may require Microsoft Excel, LibreOffice (with limited support), or conversion tools to open. If you prefer CSV, open in Excel and save as `.xlsx` or `.csv`.

How to run the notebooks:
- Install Python packages (example): pandas, numpy, matplotlib, statsmodels, scikit-learn, jupyter.
- Launch Jupyter and open `TimeSeries_ARIMA` notebook. Running the notebook top-to-bottom should reproduce analyses if the environment matches the original (same Python versions and packages).

### Task 3/

Files:
- `Task 3 - Experiments.ipynb`
	- Notebook containing experimental code and results for Task 3. Likely contains preprocessing, model training/evaluation, and result visualization.

- `Task 3 - Notes.txt`
	- Plain-text notes (observations, TODOs, or reminders) related to Task 3 experiments.

- `Task 3 - Recommendation System - Report.pdf`
	- A written report summarizing the recommendation system design, experiments and findings.

- `Task 3 - Recommendation Systems - GoogleColab.ipynb`
	- A notebook intended for execution on Google Colab. It may include data downloads and runtime-specific cells (Colab mount commands etc.). Open with Colab for best compatibility.

- `Task 3 - STC_T3 - Recommendation System.ipynb`
	- Another notebook for Task 3 (possibly the original local notebook). Inspect to see differences vs the Colab notebook.

Suggested workflow: read the Colab notebook (if you want quick execution in the cloud), then use the local notebook(s) for offline reproducibility.

## Quick reproduction tips

- Notebooks
	- Use a virtual environment (venv or conda). Example (macOS / zsh):
		- python -m venv .venv
		- source .venv/bin/activate
		- pip install -r requirements.txt  # if you have one; else install pandas, numpy, jupyter, matplotlib, seaborn, scikit-learn, statsmodels

- Excel `.xlsb`
	- Open in Excel and export to `.csv` or `.xlsx` for easier programmatic access.

- Google Colab
	- Use the provided Colab notebook(s) to run heavier cells without local dependency installation.

## Notes, assumptions & limitations

- This README documents files present in the repository at the time of writing. I did not modify any analysis files.
- The precise package list and dataset schema are not included in the repo; to fully reproduce experiments you may need to inspect each notebook's import cells and create an appropriate `requirements.txt` (I can help generate this if you want).

## Suggested next steps (optional enhancements)

1. Add a `requirements.txt` or `environment.yml` listing exact package versions used by the notebooks.
2. Add short README.md files inside each `Task` folder summarizing what to run first and any dataset paths.
3. Convert the `.xlsb` dataset to `.csv` for easier programmatic use and include a small script to load it.

---

If you'd like, I can also:
- generate a `requirements.txt` by scanning the notebooks for imports,
- add per-task README files inside each `Task` folder,
- or convert the `.xlsb` to `.csv` for you (I can attempt it here if you want).

If you'd like any of those, tell me which and I'll add them next.

# STV-TV
