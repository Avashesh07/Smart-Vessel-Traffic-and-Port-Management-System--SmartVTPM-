# Fuel Consumption Prediction for Maritime Vessels

This project aims to predict fuel consumption for various types of maritime vessels using AIS (Automatic Identification System) data. By analyzing factors like speed, course, and vessel type, this project explores machine learning approaches to predict fuel consumption, which can help the shipping industry optimize fuel usage and reduce emissions.

The motivation behind this project was to stand out in the job application process by building a project directly related to a data science role in the maritime industry. This project demonstrates my ability to understand the task requirements, work with complex datasets, and deploy machine learning solutions.

Data used in this project is sourced from [NOAA's AIS data](https://coast.noaa.gov/). It includes information on vessel type, speed, course, location, and timestamps. 


### Project Structure

- `data/`: Folder for dataset used .
- `notebooks/`: Jupyter notebooks for data exploration, feature engineering, and model training.
- `requirements.txt`: List of required Python packages.
- `README.md`: Project overview and documentation.


### Methodology
1. **Data Preprocessing**: Cleaned the data and handled missing values for key columns like vessel type.
2. **Feature Engineering**: Created new features based on domain knowledge, including time-based features and non-linear transformations of speed.
3. **Exploratory Data Analysis (EDA)**: Analyzed distributions of key variables to understand patterns and relationships.
4. **Model Training**: Trained a Random Forest model to predict fuel consumption.
5. **Model Evaluation**: Evaluated the model using Mean Squared Error (MSE) and Mean Absolute Error (MAE) and visualized predictions.
6. **Feature Importance Analysis**: Identified important features influencing fuel consumption predictions.

### Results
The Random Forest model achieved the following results on the test data:

- **Mean Squared Error**: 0.011
- **Mean Absolute Error**: 0.086

The features `SOG` and `SOG_squared` had the highest importance in predicting fuel consumption, showing the critical role of speed in fuel use for maritime vessels.

### Installation and Usage


1. Clone this repository:
```bash
   git clone https://github.com/avashesh07/fuel-consumption-prediction.git
   cd fuel-consumption-prediction
```
 
2. Install the required packages:


```bash
pip install -r requirements.txt
```
 
3. Run the Jupyter notebooks in the `notebooks/` folder to see the analysis and model training process.

### Acknowledgements
- NOAA for providing the AIS data used in this project.
- Scikit-learn for machine learning tools.

