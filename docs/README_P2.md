# P2 – Gymnastics Scores and Demographics Joined Dataset

## 1. Description
P2 combines competition score data from major 2022–2023 gymnastics events with demographic variables derived from the Athlete Events dataset.  

It enables analysis of how demographic characteristics influence competition performance.

Only athletes with complete demographic information (age, height, weight) were retained.

---

## 2. Variables

| Column         | Description |
|----------------|-------------|
| `name`         | Athlete’s full name |
| `country_code` | ISO 3166-1 alpha-3 country code |
| `age`          | Age in years |
| `height_cm`    | Height in cm |
| `weight_kg`    | Weight in kg |
| `apparatus`    | Apparatus name (FIG standard) |
| `score`        | Score achieved in competition |
| `competition`  | Name of competition |
| `year`         | Competition year |
| `round`        | Qualifying / Final (if present) |

---

## 3. Provenance

This dataset is derived from two reused datasets:

### **R1 – Athlete Events – Olympics**
- Source: Kaggle  
- URL: https://www.kaggle.com/code/jlove5/olympic-data-women-s-gymnastics  

### **R2 – Gymnastics Scores 2022–2023**
- Source: GitHub  
- URL: https://github.com/ucsas/gym2024data/blob/main/cleandata/data_2022_2023.csv  

Both datasets were accessed on: 30.10.2025.

---

## 4. Preprocessing Steps

- Loaded both datasets using Python 3.11  
- Standardised athlete names for consistency  
- Converted country names → ISO 3166-1 alpha-3  
- Normalised apparatus naming (Vault, Floor, Beam, Uneven Bars)  
- Joined R1 and R2 on `name + country_code`  
- Removed rows with missing demographic information  
- Exported the final dataset as CSV to `cleandata/`

---

## 5. File Format

- CSV, UTF-8  
- Estimated size: < 100 MB  

---

## 6. Licence

This dataset is published under the **Creative Commons Attribution 4.0 (CC BY 4.0)** licence.

---

## 7. Persistent Identifier

DOI: 10.70124/ss6ae-53p30