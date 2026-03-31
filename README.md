# Behavioral Analysis Fraud Detection

## Overview

This project performs behavioral analysis to detect fraudulent user activity.
A neural network model is trained using user behavior features and deployed through a Streamlit web interface for real-time prediction.

## Features

* Behavioral fraud detection
* Neural network model using TensorFlow
* Training accuracy and loss visualization
* Streamlit web interface
* Real-time prediction
* Google Colab deployment

## Technologies Used

* Python
* TensorFlow / Keras
* Pandas
* NumPy
* Matplotlib
* Streamlit
* Google Colab

## Dataset

The dataset contains behavioral features such as:

* Login hour
* Session duration
* Clicks
* Device change
* Failed logins
* Fraud label (target)

## Model Architecture

* Dense layer (16 neurons, ReLU)
* Dense layer (8 neurons, ReLU)
* Output layer (Sigmoid)

Loss Function: Binary Crossentropy
Optimizer: Adam

## Training

The model is trained using an 80/20 train-test split.
Training and validation accuracy and loss are plotted for evaluation.

## Prediction

The model predicts whether user behavior is:

* Normal Behavior
* Fraudulent Behavior Detected

## Streamlit Interface

The web application accepts:

* Login Hour
* Session Duration
* Clicks
* Device Changed
* Failed Logins

Based on the inputs, the system analyzes behavior and displays the prediction.

## How to Run (Google Colab)

Install Streamlit:

```
!pip install streamlit
```

Run Streamlit:

```
!streamlit run app.py &>/content/logs.txt &
```

Create Public URL:

```
!wget -q https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-linux-amd64
!chmod +x cloudflared-linux-amd64
!./cloudflared-linux-amd64 tunnel --url http://localhost:8501
```

## Output

* Normal Behavior
* Fraudulent Behavior Detected

## Future Improvements

* Model saving and loading
* Improved feature engineering
* Real-time deployment
* Cloud hosting

## Author

Behavioral Analysis Fraud Detection Project

