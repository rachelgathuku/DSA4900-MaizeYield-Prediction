# 🌾 Maize Yield Prediction using Remote Sensing and Machine Learning

## Project Overview
This project investigates maize yield prediction across major Kenyan counties using satellite-derived indices and meteorological variables. The goal is to evaluate how remote-sensing and climate data can improve the accuracy of yield forecasts, helping inform agricultural planning and food-security strategies.

The study compares a baseline Linear Regression model with an improved Random Forest (RF) model using multi-source environmental data, including NDVI, EVI, rainfall, temperature, and humidity. The models are evaluated on performance metrics such as R², RMSE, and MAE.

## Objectives
- Integrate agroclimatic and vegetation data for maize yield modeling.  
- Compare the predictive accuracy of statistical and machine learning methods.  
- Identify the most influential environmental factors driving yield variability.  
- Visualize spatial yield variability across counties in Kenya.  

## Methodology Summary
1. **Data Sources**
   - **FAOSTAT**: Historical yield data for maize (2010–2024).  
   - **NASA POWER**: Climate variables (rainfall, temperature, humidity).  
   - **EOSDA**: Satellite indices (NDVI, EVI) for vegetation health.  

2. **Modeling**
   - **Baseline**: Linear Regression.  
   - **Improved Model**: Random Forest Regressor with hyperparameter tuning.  

3. **Evaluation Metrics**
   - Coefficient of Determination (R²)  
   - Root Mean Squared Error (RMSE)  
   - Mean Absolute Error (MAE)  

## Key Results
| Model | R² | RMSE | MAE |
|-------|----|------|-----|
| Linear Regression | -0.25 | 0.18 | 0.15 |
| Random Forest | -0.05 | 0.16 | 0.14 |

- Humidity and NDVI were found to be the strongest predictors of maize yield.  
- The Random Forest model outperformed the baseline Linear Regression model slightly, showing better generalization.  
- Yield variability was most pronounced in Nairobi and Machakos counties.

## Visual Results
Key figures from the analysis include:
- `yield_box.png` — Yield variability across counties  
- `perf.png` — Model performance comparison  
- `learning_curve.png` — Learning curve for the Random Forest model  
- `feature_importance.png` — Feature importance ranking  
- `corr.png` — Correlation matrix among key variables  

## How to Run the Notebook
1. **Clone or download this repository:**
   ```bash
   git clone https://github.com/YourUsername/DSA4900-MaizeYield-Prediction.git
   cd DSA4900-MaizeYield-Prediction
   ```

2. **Open the notebook**
   - Launch Jupyter Notebook or JupyterLab.  
   - Open `Copy_of_DSA4900.ipynb`.

3. **Install dependencies (if not pre-installed):**
   ```bash
   pip install pandas numpy matplotlib scikit-learn seaborn
   ```

4. **Run all cells** sequentially to reproduce results.

## Repository Structure
```
DSA4900-MaizeYield-Prediction/
│
├── Copy_of_DSA4900.ipynb         # Main analysis notebook
├── yield_box.png                 # Yield variability plot
├── perf.png                      # Baseline vs improved performance
├── learning_curve.png            # Learning curve (RF)
├── feature_importance.png        # Feature importance bar chart
├── corr.png                      # Correlation matrix heatmap
└── README.md                     # Project overview and guide
```

## Citation
If using this project or dataset subset, please cite appropriately:
> Gathuku, R. (2025). *Maize Yield Prediction using Remote Sensing and Machine Learning*. DSA4900 Final Project, [University Name].

## Contact
**Author:** Rachel Gathuku  
**License:** MIT License (open for academic and research use)
