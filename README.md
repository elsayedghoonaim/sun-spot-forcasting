This project focuses on predicting the monthly mean total sunspot number using various machine learning models. The dataset spans from January 1749 to January 2021, containing the monthly mean total sunspot numbers. The project involves data exploration, preprocessing, model training, and evaluation using Decision Tree, XGBoost, and ARIMA models.

### Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Project Structure](#project-structure)
4. [Data Exploration & Wrangling](#data-exploration--wrangling)
5. [Data Preprocessing](#data-preprocessing)
6. [Data Splitting](#data-splitting)
7. [Baseline Readings](#baseline-readings)
8. [Models](#models)
    - [Decision Tree Model](#decision-tree-model)
    - [XGBoost Model](#xgboost-model)
    - [ARIMA Model](#arima-model)
9. [Results](#results)
10. [Contributing](#contributing)
11. [License](#license)

### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/sunspot-prediction.git
   ```
2. Navigate to the project directory:
   ```sh
   cd sunspot-prediction
   ```
3. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```

### Usage
1. Place the dataset `Sunspots.csv` in the project directory.
2. Run the Jupyter notebook `sunspot_prediction.ipynb` to execute the data exploration, preprocessing, and model training steps.

### Project Structure
- `sunspot_prediction.ipynb`: Jupyter notebook containing the project code.
- `Sunspots.csv`: Dataset file containing the monthly mean total sunspot numbers.
- `README.md`: Project documentation.
- `requirements.txt`: List of required Python packages.

### Data Exploration & Wrangling
- Load and explore the dataset to understand its structure and characteristics.
- Handle missing values and convert the `Date` column to a datetime format.
- Visualize the data to identify patterns and trends.

### Data Preprocessing
- Create lagged features to include past sunspot numbers as predictors.
- Prepare the dataset for model training by creating features and target variables.

### Data Splitting
- Split the dataset into training and testing sets using an 80-20 split.

### Baseline Readings
- Calculate the baseline mean absolute error (MAE) using the mean of the training set as the prediction.

### Models
#### Decision Tree Model
- Train a Decision Tree Regressor on the training data.
- Evaluate the model using mean absolute error (MAE) on the test data.

#### XGBoost Model
- Train an XGBoost Regressor on the training data.
- Evaluate the model using mean absolute error (MAE) on the test data.

#### ARIMA Model
- Perform hyperparameter tuning for the ARIMA model.
- Evaluate the model using mean absolute error (MAE) on the test data.

### Results
- Compare the performance of the different models using mean absolute error (MAE).
- Visualize the predictions of each model against the actual values.

### Contributing
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
