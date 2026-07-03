Smile Stalker - Image Smile Detection App

A Streamlit web application that detects smiles in uploaded images using a pre-trained logistic regression model.

🚀 Features

Image Upload: Support for JPG, PNG, and JPEG formats

Real-time Processing: Instant smile detection on uploaded images

Confidence Scoring: Visual slider showing smile detection confidence percentage

User-Friendly Interface: Clean and intuitive web interface

Pre-trained Model: Uses a trained logistic regression classifier

🛠️ Installation

Clone this repository:

git clone <https://github.com/sow-bharani/Smile-Stalker---Image-Smile-Detection-App.git>
cd smile-stalker

Install required dependencies:

pip install streamlit numpy scikit-learn joblib pillow

📦 Dependencies

streamlit - Web application framework

numpy - Numerical computations

scikit-learn - Machine learning utilities

joblib - Model serialization

PIL (Pillow) - Image processing

🎯 Usage

Run the Streamlit app:

streamlit run app.py

Open your web browser and go to http://localhost:8501

Upload an image using the file uploader

View the results:

Uploaded image preview

Smile score slider (0-100%)

Classification result (smiling or not smiling)

Confidence percentage

🔧 How It Works

Image Preprocessing:

Converts image to grayscale

Resizes to 64x64 pixels

Flattens image to 1D array

Applies standard scaling

Model Prediction:

Uses pre-trained logistic regression model

Calculates probability of smiling

Returns binary classification with confidence score

📁 Project Structure

smile-stalker/
├── app.py                 # Main Streamlit application
├── smile_stalker.pkl     # Pre-trained model (not included in repo)
├── scaler.pkl           # Fitted scaler (not included in repo)
├── requirements.txt     # Python dependencies
└── README.md           # Project documentation

🎮 Model Details

Algorithm: Logistic Regression

Input Size: 64x64 grayscale images (4096 features)

Output: Binary classification (smiling/not smiling) with probability score

Preprocessing: StandardScaler for feature normalization

⚠️ Note

The model files (smile_stalker.pkl and scaler.pkl) are not included in this repository. You'll need to:

Train your own model using a smile detection dataset

Save the model and scaler using joblib

Update the file paths in the load_model() function

🔮 Future Enhancements

Support for real-time webcam smile detection

Batch image processing

Model performance metrics

Different model architectures (CNN, etc.)

Export functionality for results

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check issues page.

