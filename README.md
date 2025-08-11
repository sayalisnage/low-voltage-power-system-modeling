# Low-Voltage Level Power System Modelling  
**Forecasting Energy Consumption and Maximum Demand**

A data science project aimed at analyzing and forecasting energy consumption and peak demand in residential and small commercial low-voltage systems. Using detailed time series data collected from households in Southern Germany, this project investigates load characteristics, seasonal and daily energy patterns, and evaluates multiple regression models to predict energy demand and improve energy efficiency.

---

## Project Overview

Energy consumption and maximum demand forecasting are crucial for enhancing energy efficiency and planning reliable power systems. This project focuses on studying the consumption patterns of connected electrical loads in households and small businesses, aiming to build robust models that predict maximum electricity demand. By analyzing these patterns and forecasting future demand, the project contributes to energy sustainability and cost reduction.

---

## Data Sources

* **Open Power System Data:** Time series electricity consumption data from 11 households in Southern Germany, spanning 2014 to 2020.
  * Includes 15-minute and 60-minute interval datasets.
  * Features: total energy consumption, photovoltaic (PV) generation, electric vehicle charging, energy import/export, and appliance-level consumption.
  * Source: [https://open-power-system-data.org/](https://open-power-system-data.org/)

---

## Methodology

* **Data Cleaning and Preparation:**  
  - Standardized column names and formats, removed duplicates and irrelevant columns.  
  - Filtered data to December 2015 through June 2017.  
  - Imputed missing values and aggregated energy features such as total PV generation and hourly maximum demand.

* **Feature Engineering & Dimensionality Reduction:**  
  - Correlation analysis to identify features highly associated with maximum demand.  
  - Applied Principal Component Analysis (PCA) to reduce feature dimensionality while preserving 90% of variance.  
  - Split data into training (80%) and testing (20%) sets.

* **Model Development and Evaluation:**  
  - Trained various regression models including Simple Linear Regression, Ridge, Lasso, Elastic Net, K-Nearest Neighbors (KNN), Decision Tree, Random Forest, and Gradient Boosting.  
  - Evaluated models using R², Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).  
  - Compared models to identify the best predictors for maximum demand.

---

## Results

* Gradient Boosting, K-Nearest Neighbors, and Random Forest models achieved the highest accuracy with R² values around 0.99, indicating excellent predictive capability.  
* PCA improved model reliability by mitigating overfitting present in simpler models.  
* A strong correlation was observed between appliance-level energy consumption and overall maximum demand.

---

## Limitations

* Dataset is geographically limited to Southern Germany, which may affect generalizability.  
* External factors such as weather conditions, appliance specifications, and tariff changes were not fully incorporated.  
* The impact of climate variability and unforeseen events (e.g., load shedding) introduces uncertainties not captured in models.

---

## Ethical Considerations

Energy consumption patterns reflect not only technical and economic aspects but also social and environmental equity. This project acknowledges the importance of privacy in household data collection and supports policies aimed at equitable and sustainable energy use.

---

## Technology Stack

* **Programming Language:** Python  
* **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
* **Tools:** Jupyter Notebook  

---

## Future Work

* Integrate meteorological and tariff data for enhanced forecasting accuracy.  
* Develop a real-time dashboard for monitoring and predicting energy consumption.  
* Expand analysis to broader geographic regions for improved applicability.  
* Investigate advanced modeling techniques such as deep learning architectures.

---

## Contact

For questions or collaboration, please reach out via [E-mail](mailto:sayalinage@gmail.com) or connect on [LinkedIn](https://www.linkedin.com/in/sayali-nage-34303b136/).

---
