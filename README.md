# Multiple Disease Prediction System

A comprehensive machine learning web application built with Streamlit that predicts three different diseases using trained ML models. The system provides an intuitive interface for healthcare professionals and individuals to assess disease risk based on medical parameters.

## 🏥 Diseases Covered

### 1. Diabetes Prediction

Predicts the likelihood of diabetes based on 8 key medical parameters:

- Number of Pregnancies
- Glucose Level
- Blood Pressure Level
- Skin Thickness Value
- Insulin Value
- BMI (Body Mass Index)
- Diabetes Pedigree Function Value
- Age

### 2. Heart Disease Prediction

Assesses heart disease risk using 13 cardiovascular parameters:

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Serum Cholesterol (mg/dl)
- Fasting Blood Sugar > 120 mg/dl
- Resting Electrocardiographic Results
- Maximum Heart Rate Achieved
- Exercise Induced Angina
- ST Depression Induced by Exercise
- Slope of Peak Exercise ST Segment
- Major Vessels Colored by Fluoroscopy
- Thalassemia (0 = normal; 1 = fixed defect; 2 = reversible defect)

### 3. Parkinson's Disease Prediction

Detects Parkinson's disease using 22 voice measurement parameters:

- MDVP:Fo(Hz) - Average vocal fundamental frequency
- MDVP:Fhi(Hz) - Maximum vocal fundamental frequency
- MDVP:Flo(Hz) - Minimum vocal fundamental frequency
- MDVP:Jitter(%) - Percentage jitter
- MDVP:Jitter(Abs) - Absolute jitter
- MDVP:RAP - Relative amplitude perturbation
- MDVP:PPQ - Five-point period perturbation quotient
- Jitter:DDP - Average absolute difference of differences between jitter cycles
- MDVP:Shimmer - Multi-dimensional voice perturbation shimmer
- MDVP:Shimmer(dB) - Shimmer in dB
- Shimmer:APQ3 - Three-point amplitude perturbation quotient
- Shimmer:APQ5 - Five-point amplitude perturbation quotient
- MDVP:APQ - 11-point amplitude perturbation quotient
- Shimmer:DDA - Average absolute differences between the amplitudes of consecutive periods
- NHR - Noise-to-harmonics ratio
- HNR - Harmonics-to-noise ratio
- RPDE - Recurrence period density entropy
- DFA - Detrended fluctuation analysis
- spread1, spread2 - Nonlinear dynamical complexity measures
- D2 - Correlation dimension
- PPE - Pitch period entropy

## ⚙️ Technology Stack

- **Frontend**: Streamlit
- **Machine Learning**: Scikit-learn
- **Data Processing**: NumPy, Pandas
- **Model Persistence**: Pickle
- **UI Components**: streamlit-option-menu

## 🚀 Installation & Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/Abbasam8910/Public-ML-Web-App.git
   cd Public-ML-Web-App
   ```

2. **Install required dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**

   ```bash
   streamlit run "Multiple Disease Predictor.py"
   ```

4. **Access the application**
   Open your web browser and navigate to `http://localhost:8501`

## 📁 Project Structure

```
Public-ML-Web-App/
├── Multiple Disease Predictor.py    # Main Streamlit application
├── trained_model.sav               # Diabetes prediction model
├── heart_disease_model.sav         # Heart disease prediction model
├── parkinsons_model.sav           # Parkinson's disease prediction model
├── requirements.txt               # Python dependencies
├── README.md                     # Project documentation
└── LICENSE                      # License file
```

## 🎯 How to Use

1. **Launch the application** using the installation steps above
2. **Select a disease** from the sidebar menu:
   - Diabetes Prediction
   - Heart Disease Prediction
   - Parkinson's Prediction
3. **Enter the required parameters** in the input fields
4. **Click the prediction button** to get results
5. **View the prediction result** displayed on the screen

## 🧠 Machine Learning Models

The application uses pre-trained machine learning models saved as pickle files:

- **Diabetes Model** (`trained_model.sav`): Trained on diabetes dataset with 8 features
- **Heart Disease Model** (`heart_disease_model.sav`): Trained on heart disease dataset with 13 features
- **Parkinson's Model** (`parkinsons_model.sav`): Trained on Parkinson's dataset with 22 voice features

## 📊 Features

- **Multi-Disease Prediction**: Three different disease prediction models in one application
- **User-Friendly Interface**: Clean and intuitive Streamlit-based web interface
- **Real-Time Predictions**: Instant results upon clicking prediction buttons
- **Responsive Design**: Works well on different screen sizes
- **Easy Navigation**: Sidebar menu for switching between different prediction models

## ⚠️ Disclaimer

This application is for educational and informational purposes only. The predictions should not be considered as professional medical advice. Always consult with qualified healthcare professionals for proper medical diagnosis and treatment.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the terms specified in the LICENSE file.

## 👨‍💻 Developer

Created by [Abbasam8910](https://github.com/Abbasam8910)

---

**Note**: Make sure all model files (`.sav` files) are present in the project directory before running the application.
