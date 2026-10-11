# AI Predictive Maintenance for Industrial Machinery

## Project Overview

This project applies machine learning to industrial predictive maintenance, with the goal of identifying early warning signs of equipment degradation and supporting data-driven maintenance planning. It is designed for industrial equipment such as centrifugal pumps and gas turbines.

The model uses equipment operating conditions, temperature, pressure, vibration, lubrication indicators, maintenance history, and equipment health indicators to support predictive maintenance analysis.

The project combines mechanical engineering knowledge with artificial intelligence to explore how data-driven tools can help improve equipment reliability, reduce unplanned downtime, and support maintenance decision-making.

## Objectives

- Identify operating patterns associated with potential equipment faults.
- Explore early warning indicators of machinery degradation.
- Support maintenance planning using equipment condition data.
- Investigate remaining useful life (RUL) prediction.
- Develop a foundation for a machine learning-based predictive maintenance application.

## Features and Input Variables

The model's feature list includes:

| Category | Example variables |
|---|---|
| Operating conditions | Operating hours, load percentage, RPM |
| Pressure and temperature | Suction pressure, discharge pressure, bearing temperature |
| Vibration monitoring | Axial vibration, radial vibration, overall vibration |
| Lubrication | Oil pressure, oil temperature, oil debris count |
| Performance | Flow rate, motor power, efficiency |
| Maintenance history | Days since maintenance, maintenance count |
| Equipment health | Degradation index, health index |
| Equipment information | Equipment type and fault mode |

The saved feature list also contains target-related fields such as `failure_next_7d` and `rul_hours`. These must be handled appropriately when preparing model inputs to prevent data leakage.

## Technology Stack

- **Python** — data processing and model integration
- **Pandas and NumPy** — data manipulation
- **Scikit-learn** — machine learning
- **Joblib/Pickle** — model serialization and loading
- **Streamlit** — potential interactive web application
- **Google Colab** — model development and experimentation
- **GitHub** — version control and project documentation

## How It Works

1. **Data collection:** Obtain machinery operating measurements, condition-monitoring records, and maintenance history.
2. **Data preprocessing:** Handle missing values, check data quality, encode categorical variables, and prepare model inputs.
3. **Model inference:** Pass correctly ordered and preprocessed input features to the saved model.
4. **Prediction:** Generate the output supported by the trained model, such as a fault classification or failure-risk estimate.
5. **Maintenance decision support:** Use the prediction alongside engineering inspections, operating limits, and maintenance procedures.

## Model Artifacts

The repository includes the following artifacts:

- `machinery_predictive_maintenance_model.pkl` — serialized machine learning model.
- `machinery_model_features.pkl` — saved list of model feature names and their expected order.

**Important:** The actual model type, target variable, validation scores, and prediction outputs should be confirmed from the training pipeline before being documented as established results.

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

Install the required packages:

```bash
pip install pandas numpy scikit-learn joblib streamlit
```

Use the package versions compatible with the saved model and its training environment.

## Potential Applications

- Industrial pump condition monitoring
- Compressor and gas turbine maintenance
- Equipment degradation analysis
- Maintenance prioritization
- Remaining useful life research
- Data-driven reliability engineering

## Limitations

Model predictions depend on data quality, representative training data, and appropriate validation. Synthetic or simulated data can support development, but real industrial deployment requires validation against representative equipment data. Predictions should complement—not replace—engineering inspection, safety procedures, and manufacturer recommendations.

## Future Improvements

- Build an interactive Streamlit dashboard.
- Add fault-risk visualizations and equipment health indicators.
- Validate performance on unseen test data and real equipment records.
- Report suitable classification or regression metrics.
- Add model monitoring and prediction logging.
- Explore integration with industrial sensors and maintenance databases.

## Author

Mechanical Engineering | Machinery Maintenance | Energy Systems | Data Analytics & Data Governance |Machine Learning | Predictive Analytics

This project explores the application of artificial intelligence to industrial equipment reliability and intelligent maintenance planning.

## Disclaimer

This project is intended for research, learning, and decision-support development. It is not a certified industrial safety or fault-detection system.

