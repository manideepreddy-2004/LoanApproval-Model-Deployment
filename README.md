# LoanApproval-Model-Deployment
Premium Loan Status Predictor 
A web app built with Streamlit to predict loan approval status using a K-Nearest Neighbors machine learning model trained on loan application data.

Features
User-friendly Streamlit interface for inputting loan application features

Preprocesses categorical and numerical data with encoders and scalers

Predicts loan approval status with an accurate KNN model (~88.5% accuracy)

Theme customizations with gradient colors and clean UI

Loads and uses saved ML artifacts: model, scaler, encoders, and feature order

Setup
Requirements
Python 3.x

Install dependencies via:

text
pip install -r requirements.txt
Run Locally
text
streamlit run app.py
Project Structure
app.py: Streamlit app frontend and prediction logic

Model_Building.ipynb: Jupyter notebook for data preprocessing, model training, evaluation, and saving artifacts

model.pkl, scaler.pkl, label_encoders.pkl, feature_order.pkl, etc.: Pretrained model and data transformers

requirements.txt: Python package dependencies

space.yaml: Configuration for deploying the app with HuggingFace Spaces

Model Details
Dataset: Loan approval dataset with features preprocessed into categorical and numerical columns

Model: KNeighborsClassifier with 5 neighbors

Metrics: Achieves approximately 88.5% accuracy on the test set

Preprocessing: Label encoding for categories, MinMax scaling for numericals

Usage
Enter loan application details in the web form inputs

The app processes inputs in the required feature order, performs encoding and scaling, then predicts the loan status

The predicted result is displayed instantly
