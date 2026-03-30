# PPHA 30538 Final Project: The Cycle of Disinvestment


## Data Sources

Several datasets exceed GitHub's 100MB file size limit and are hosted externally. Download each file and place it in `dataset/raw/` before running any code.

| Dataset | Source | Access |
|---|---|---|
| Chicago Outstanding Debt (365+ Days) | Department of Finance, Chicago Mayor's Office | [Download](https://docs.google.com/spreadsheets/d/11rmLkfwTM4J62-yavqgpoTUvKEGKAFVI/edit?usp=drive_link&ouid=103252786202124037419&rtpof=true&sd=true) |
| Chicago Demolition Permits | Chicago Data Portal | [Download](https://drive.google.com/file/d/1R-_NtNpnVFif8eztaej20XMxue5Dhdb8/view?usp=drive_link) |
| Cook County Parcel Universe | Cook County Assessor's Office | [Download](https://datacatalog.cookcountyil.gov/Property-Taxation/Assessor-Parcel-Universe-Current-Year-Only-/pabr-t5kh/about_data) |
| Chicago Vacant Land Parcels | Cook County Assessor's Office | [Download](https://drive.google.com/file/d/1G8XQ3b05Bop3aKWlFnMmdBDZsP0-rXJ-/view?usp=drive_link), [classcode guide](https://prodassets.cookcountyassessoril.gov/s3fs-public/form_documents/classcode.pdf)|

> **Note:** Files should be saved to `dataset/raw/` without renaming. File paths in `preprocessing.py` are set up accordingly.

## Streamlit App

The interactive dashboard is deployed at: [https://ward-level-debt.streamlit.app]

Running the Streamlit Dashboard

The interactive dashboard is deployed using Streamlit.

If the app has not been accessed in the last 24 hours, Streamlit automatically puts it to sleep to conserve resources. When this happens, the app may take 30–60 seconds to “wake up” after you open the link.

If the page appears blank or slow to load initially, please wait a moment while the app starts up. Once it wakes up, the dashboard should load normally.

## Repository Structure

```
├── .github/
│   └── workflows/
│       └── keep-streamlit-alive.yml  # GitHub Actions workflow to keep app awake
├── Presentation/             # Slide deck
├── code/cleaning/            # Data cleaning scripts
├── data/                     # Processed data files
├── streamlit-app/            # Dashboard code and dependencies
├── final_project.qmd         # Writeup source file
├── final_project.html        # Rendered writeup
├── final_project.pdf         # Rendered writeup (PDF)
├── requirements.txt          # Python dependencies
└── README.md
```
