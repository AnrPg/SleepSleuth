# SleepSleuth

> A comprehensive pipeline for analyzing lifestyle and physiological factors affecting sleep health, using statistical, visual, and machine learning techniques to profile sleep disorders — all inside Google Colab.

![Python](https://img.shields.io/badge/python-3.8+-blue)
![Bioinformatics](https://img.shields.io/badge/domain-bioinformatics-green)
![Platform](https://img.shields.io/badge/platform-Google_Colab-orange)

---

## 📖 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [How to Use (Colab)](#-how-to-use-colab)
- [Input/Output](#-inputoutput)
- [Example](#-example)
- [Dependencies](#-dependencies)
- [Project Structure](#-project-structure)
- [License](#-license)
- [Citations](#-citations)
- [Contact](#-contact)

---

## 🧬 Overview

This project analyzes the **Sleep Health and Lifestyle Dataset**, aiming to identify correlations between daily habits and the presence of sleep disorders. It applies **statistical modeling, visualization, and data preprocessing** workflows to uncover patterns related to insomnia and sleep apnea, integrating foundational methods in **biostatistics and biomedical data science**.

---

## ✨ Features

- [x] No installation required - runs entirely in Google Colab
- [x] Preprocessing: interpolation, encoding & normalization
- [x] Multi-method correlation analysis (Spearman, Cramér’s V, ANOVA, etc.)
- [x] Distribution profiling via skewness & kurtosis
- [x] Data visualization: heatmaps, histograms, box plots
- [x] Sleep disorder classification and pattern recognition

---

## ▶️ How to Use (Colab)

1. Open the notebook `SleepSleuth.ipynb` in Google Colab.
2. Run the first cell to mount your Google Drive:
    ```python
    from google.colab import drive
    drive.mount('/content/drive')
    ```
3. Upload `Sleep_health_and_lifestyle_dataset.csv` to your Drive (adjust the folder path in the notebook if needed).
4. Run the notebook cells step by step to analyze and visualize the data.

---

## 📥 Input/Output

**Input**:  
CSV file (`Sleep_health_and_lifestyle_dataset.csv`) with 374 rows × 13 columns, including demographics, physiological metrics, lifestyle habits, and sleep disorder presence.

**Output**:  
- Correlation matrix heatmaps
- Distribution plots
- Summary statistics
- Cleaned and encoded dataframe
- Optional saved reports in CSV or JSON

---

## 📊 Example

```python
from sleepsleuth.preprocessing import clean_data
from sleepsleuth.stats import analyze_correlations
import pandas as pd

df = pd.read_csv("Sleep_health_and_lifestyle_dataset.csv")
df_clean = clean_data(df)
cor_matrix = analyze_correlations(df_clean)
```

## 🪪 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 📬 Contact

**Author**: Apostolos-Nikolaos Rigas  
📧 regas.apn@gmail.com  
🏫 [Democritus University of Thrace – MSc Bioinformatics](https://bioinfo.mbg.duth.gr/)  
🔗 [LinkedIn](https://linkedin.com/in/apostolos-regas-1908a7239)  
🔗 [GitHub](https://github.com/AnrPg)

---

co-author: [Biosteve](https://github.com/Biosteve) (LinkedIn: in/stefanos-fragkoulis-333341205 )
