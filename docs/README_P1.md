# P1 – Cleaned Olympic Women's Gymnastics Dataset

## 1. Description
P1 is a cleaned and filtered subset of the Athlete Events dataset from Kaggle.  
It contains **only female artistic gymnastics medallists** and includes an additional derived variable indicating the scoring era:

- **"perfect10"** (all Olympics **before 2008**)
- **"openEnded"** (Olympics **2008 and later**)

This dataset enables comparisons across scoring eras and demographic patterns among top-performing gymnasts.

---

## 2. Variables

| Column         | Description |
|----------------|-------------|
| `name`         | Athlete’s full name (string) |
| `gender`       | Biological gender (“F”) |
| `age`          | Age at time of competition (years) |
| `height_cm`    | Height in centimetres |
| `weight_kg`    | Weight in kilograms |
| `team`         | Athlete’s national team (string) |
| `country_code` | ISO 3166-1 alpha-3 country code |
| `year`         | Olympic year (YYYY) |
| `event`        | Event (e.g., Team, All-Around) |
| `medal`        | Gold, Silver, Bronze |
| `era`          | “perfect10” or “openEnded” |

---

## 3. Provenance

Derived from the reused dataset:

**Athlete Events – Olympics**  
- Source: Kaggle  
- URL: https://www.kaggle.com/code/jlove5/olympic-data-women-s-gymnastics  
- Accessed: 30.10.2025 
- Licence: Apache 2.0 open source license

---

## 4. Preprocessing Steps

- Filtered data to include:
  - only “Women’s Artistic Gymnastics”
  - only medallists (Gold/Silver/Bronze)
- Standardised country names → ISO 3166-1 alpha-3 format
- Cleaned inconsistent name fields
- Converted height/weight to consistent units  
- Added derived column `era` to indicate scoring system
- Removed any athletes with missing essential demographic data

---

## 5. File Format

- CSV, UTF-8 encoding  
- Estimated size: < 100 MB  

---

## 6. Licence

This dataset is published under the **Creative Commons Attribution 4.0 (CC BY 4.0)** licence.

---

## 7. Persistent Identifier

DOI: 