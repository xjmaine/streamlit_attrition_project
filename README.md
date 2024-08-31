# Employee Attrition Prediction

This project aims to predict employee attrition using machine learning techniques. The application provides an interactive interface built with Streamlit, allowing users to input various features related to employee demographics, work information, and satisfaction indices to receive predictions about their likelihood of attrition.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Data Preprocessing](#data-preprocessing)
- [Model Training](#model-training)
- [Web Application](#web-application)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The project consists of the following main components:

1. **Data Preprocessing**: Cleaning and preparing the dataset for modeling.
2. **Model Training**: Training a machine learning model to predict employee attrition.
3. **Web Application**: An interactive web application built with Streamlit for user input and predictions.

## Technologies Used

- Python
- Streamlit
- Scikit-learn
- Pandas
- Joblib
- NumPy
- Jupyter Notebook (for experimentation)

## Data Preprocessing

The data preprocessing steps include:

- Converting data types and handling missing values.
- Encoding categorical variables using `OneHotEncoder`.
- Scaling numerical features using `StandardScaler`.

## Model Training

A Random Forest Classifier is used to predict employee attrition. The model is trained on a dataset containing employee information and their attrition status. The trained model, along with the encoder and scaler, is saved using `joblib` for later use in the Streamlit application.

## Web Application

The Streamlit application consists of several pages:

1. **Home Page**: A welcome message and overview of the application.
2. **View Data**: Displays the dataset for exploration.
3. **Predict Page**: Users can input their information and receive predictions about attrition.
4. **History Page**: Displays the history of predictions made (to be implemented).

### Predict Page Features

- Input fields are organized into three columns for better usability.
- Users can input personal information, work-related data, and satisfaction indices.
- The application provides a prediction based on the input data.

## Installation

To set up the project locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/xjmaine/streamlit_attrition_project.git

2. Navigate to the project directory:
    cd employee-attrition-prediction

3. Create a virtual environment (optional but recommended):
    python -m venv venv

4. Activate the virtual environment:
    On Windows:
    venv\Scripts\activate
    alternative: py -m streamlit run app.py

    On macOS/Linux:
    source venv/bin/activate
    alternative: py -m streamlit run app.py

5. Install the required packages:
    pip install -r requirements.txt

Usage
To run the Streamlit application, execute the following command in your terminal:
    streamlit run app.py

This will start the Streamlit server and open the application in your web browser.

Contributing
Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for more details.