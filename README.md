# House Price Prediction Using Linear Regression 🏠📈

A beginner-friendly Machine Learning project that predicts house prices based on property size using Linear Regression from Scikit-learn.

## Description

This project trains a Linear Regression model using sample house sizes and their corresponding prices. After training, the model predicts the price of a house based on its size.

This is one of the most popular beginner projects for learning:

- Machine Learning
- Predictive Analytics
- Linear Regression
- Data Modeling with Scikit-learn

## Requirements

Install the required libraries before running the project:

```python
!pip install scikit-learn numpy
```

Or from the terminal:

```bash
pip install scikit-learn numpy
```

## Code

```python
from sklearn.linear_model import LinearRegression
import numpy as np

sizes = np.array([[10000], [15000], [20000], [25000]])
prices = np.array([1000000, 1500000, 2000000, 2500000])

model = LinearRegression()
model.fit(sizes, prices)

size = [[20000]]

prediction = model.predict(size)

print("Predicted Price:", prediction[0])
```

## How to Run

1. Install Python 3.
2. Install the required libraries:

```bash
pip install scikit-learn numpy
```

3. Save the code as `house_price_prediction.py`.
4. Run the program:

```bash
python house_price_prediction.py
```

## Example

### Training Data

| House Size (sq ft) | Price |
|-------------------|--------:|
| 10,000 | 1,000,000 |
| 15,000 | 1,500,000 |
| 20,000 | 2,000,000 |
| 25,000 | 2,500,000 |

### Input

```python
size = [[20000]]
```

### Output

```text
Predicted Price: 2000000.0
```

## Features

- Predicts house prices based on size
- Uses Linear Regression
- Simple and easy-to-understand dataset
- Beginner-friendly AI/ML project
- Demonstrates supervised learning

## Concepts Used

### NumPy

Used to create and manage numerical datasets.

```python
import numpy as np
```

### Linear Regression

Linear Regression finds the relationship between:

```text
House Size → House Price
```

and predicts future values based on that relationship.

### Model Training

```python
model.fit(sizes, prices)
```

The model learns patterns from the provided data.

### Prediction

```python
prediction = model.predict(size)
```

The trained model estimates the price for a new house size.

## Machine Learning Workflow

```text
Training Data
      ↓
Linear Regression Model
      ↓
Model Training
      ↓
Prediction
      ↓
Estimated House Price
```

## Project Structure

```text
house-price-prediction/
│
├── house_price_prediction.py
└── README.md
```

## Future Improvements

- Use larger real-world datasets
- Add multiple features (bedrooms, bathrooms, location)
- Visualize data with Matplotlib
- Save and load trained models
- Build a web application using Flask or Streamlit
- Evaluate model accuracy using metrics like R² Score and MAE

## Sample Advanced Dataset

```python
sizes = np.array([
    [1000],
    [1200],
    [1500],
    [1800],
    [2200],
    [2500]
])

prices = np.array([
    100000,
    120000,
    150000,
    180000,
    220000,
    250000
])
```

Using more data generally improves prediction quality.

## License

This project is open source and free to use.
