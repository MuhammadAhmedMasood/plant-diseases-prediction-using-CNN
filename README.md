# plant-diseases-prediction-using-CNN
The model uses a Convolutional Neural Network (CNN) to classify plant leaf images into 38 different disease categories. Users can upload an image, and the app predicts the disease based on the trained CNN model.

This repository contains a Streamlit app and a Convolutional Neural Network (CNN) model to classify plant leaf images into 38 different disease categories. Users can upload an image to check which disease the plant might have.

The app can be run:

Locally using Streamlit (main.py)

Dockerized using the provided Docker setup

Files Included

main.py – Streamlit app to upload images and predict disease.

Dockerfile – For building a Docker image of the app.

config.toml & credentials.toml – Configuration files for Docker deployment.

requirements.txt – Lists Python libraries needed.

plant_disease_prediction_using_cnn.py – Python script used to train the CNN model (developed in Google Colab).

class_indices.json – Mapping of class names to numeric labels, required for prediction.

Installation & Usage
Run Locally

Clone the repository:

git clone https://github.com/YOUR_USERNAME/plant-disease-streamlit.git
cd plant-disease-streamlit


Install dependencies:

pip install -r requirements.txt


Run the Streamlit app:

streamlit run main.py

Run with Docker

Build the Docker image:

docker build -t plant-disease-app .


Run the Docker container:

docker run -p 8501:80 plant-disease-app


Open the app in a browser at: http://localhost:8501

Notes

The class_indices.json file is required for mapping predictions to class labels.

The CNN model was trained in Google Colab and can be retrained using plant_disease_prediction_using_cnn.py.

### Note on Model File

The trained CNN model (`plant_disease_model.h5`) is too large to include directly in the repository (50 MB).  
You can use the plant_disease_prediction_using_cnn.py to get the trained model.

