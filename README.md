# University Research Project: Influence of demographic characteristics in the sport of gymnastics (data and code)

## 1. Project Overview
This project investigates how demographic characteristics of female artistic gymnasts (such as age, height, weight, and nationality) relate to their performance outcomes. The analysis focuses on Olympic medallists across different scoring eras as well as international competition results from 2022–2023.

Two external datasets were reused and processed to produce two cleaned datasets:

- **P1 – Cleaned Olympic Gymnastics Athlete Events**  
  (female artistic gymnastics medallists + scoring-era classification)

- **P2 – Gymnastics Scores and Demographics Joined Dataset**  
  (2022–2023 competition scores joined with demographic information)

The project aims to support transparent, FAIR data practices, reproducibility, and reuse.

Produced datasets and source code are available with documentation under the following DOI persistent identifier: 10.70124/ss6ae-53p30.

---

## 2. Folder Structure

```
/rawdata/          Original raw datasets (not redistributed; accession information included)
/cleandata/        Produced datasets P1 and P2 (CSV)
/notebooks/        Jupyter Notebook used for preprocessing and joining
/docs/             README files, metadata.json, licenses, DMP
```

---

## 3. Software Requirements

This project requires the following software environment:

- **Python 3.11+**
- Jupyter Notebook
- pandas
- numpy
- matplotlib

To install all dependencies:

This project uses the **uv** package manager to ensure a fully reproducible Python environment.

To reproduce the environment, install **uv** by:

```bash
pip install uv
```

Then run:

```bash
uv sync
```

This command will:
- create a virtual environment (if none exists),
- install all required dependencies from `pyproject.toml`,
- ensure version-locked, reproducible installations.

---

## 4. How to Reproduce the Produced Datasets

1. Download the reused datasets and place them in a `rawdata/` folder:
   - Athlete Events – Olympics dataset from Kaggle  
   - Gymnastics Scores 2022–2023 dataset from GitHub  

2. Open the notebook:

```
notebooks/data_processing.ipynb
```

3. Run all cells.  
   The notebook will:
   - load and clean the Athlete Events data → create **P1**  
   - join demographic data with scores → create **P2**  
   - export both as CSV files into `cleandata/`

No manual editing is required; executing the notebook fully regenerates both datasets.

---

## 5. Provenance of Reused Datasets

### **R1 – Athlete Events – Olympics**  
- Source: Kaggle  
- URL: https://www.kaggle.com/code/jlove5/olympic-data-women-s-gymnastics  
- Licence: Apache 2.0 open source license 
- Accessed on: 30.10.2025 
- Description: Historical dataset containing athlete-level demographic and event participation information for multiple Olympic Games.

### **R2 – Gymnastics Scores 2022–2023**  
- Source: GitHub  
- URL: https://github.com/ucsas/gym2024data/blob/main/cleandata/data_2022_2023.csv  
- Licence: no information available  
- Accessed on: 30.10.2025  
- Description: Competition scores from major artistic gymnastics events including European and World Championships.

---

## 6. Licensing

- **Produced datasets (P1, P2):** CC-BY 4.0  
- **Source code:** MIT License  
- **Reused datasets:** Not redistributed; referenced only via URLs.

---

## 7. Citation

If using this work, please cite.