# Urban Road Accident Risk and Hotspot Prediction Using Predictive Analytics

## Overview
This project focuses on analyzing road accident data using machine learning techniques to predict accident severity and identify high-risk locations (hotspots).

Traditional approaches rely mainly on accident frequency, which does not fully capture risk. This project introduces a **risk-based approach** by combining accident severity and frequency to identify critical locations more effectively.

---

## Dataset
The dataset used in this project is obtained from the **UK Department for Transport (DfT)** road safety open data.

* **Dataset Link:** [DfT Road Casualty Statistics (Last 5 Years)](https://data.dft.gov.uk/road-accidents-safety-data/dft-road-casualty-statistics-collision-last-5-years.csv)
* **Key Features:**
    * **Accident Severity:** (Slight, Serious, Fatal)
    * **Geographic Location:** Latitude, Longitude
    * **Time Information:** Date, Hour, Day, Month
    * **Environmental Conditions:** Weather, Lighting, Road Surface

> **Note:** The dataset is not included in this repository due to its large size (~94 MB).

---

## Methodology
The project follows a structured workflow to move from raw data to actionable risk insights:

1.  **Data Preprocessing:** Cleaning and handling missing values.
2.  **Feature Engineering:** Selection of key variables and encoding categorical data.
3.  **Class Imbalance Handling:** Implementing oversampling techniques to ensure severe accidents are accurately predicted.
4.  **Model Training:** Evaluating multiple algorithms including:
    * Logistic Regression
    * Random Forest
    * XGBoost
5.  **Risk Analysis:**
    * Hotspot identification using a **composite risk score**.
    * Spatial, temporal, and environmental analysis.

---

## Key Results
* **Class Imbalance:** Significant imbalance exists; models trained without adjustment fail to detect severe accidents.
* **Oversampling Impact:** Performance improved significantly after balancing the dataset.
* **Best Model:** **Random Forest** provided the most balanced performance across all metrics.
* **Hotspot Insights:** High-risk hotspots are **not always** the locations with the highest frequency of accidents; severity weighting changes the priority map.

---

## Technologies Used
* **Language:** Python
* **Data Libraries:** Pandas, NumPy
* **Visualization:** Matplotlib
* **Machine Learning:** Scikit-learn, XGBoost

---

## How to Run
1.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
2.  **Open the notebook:**
    Open `Urban_Road_Accident_Risk_and_Hotspot_Prediction_Using_Predictive_Analytics.ipynb` in Jupyter or VS Code.
3.  **Execution:**
    Run all cells sequentially to reproduce the analysis.

---

## Repository Structure
| File | Description |
| :--- | :--- |
| `Urban_Road_Accident_Risk_and_Hotspot_Prediction_Using_Predictive_Analytics.ipynb` | Main analysis and modeling notebook |
| `Urban_Accident_Risk_Report.docx` | Comprehensive project report |
| `requirements.txt` | List of necessary Python packages |
| `README.md` | Project documentation |

---

## Author
**Yuvaraj U** VIT, Chennai
