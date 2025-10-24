# Cancer Survival Prediction Companion

## 📋 Table of Contents
- [Project Overview](#-project-overview)
- [How It Works](#-how-it-works)
- [Technologies Used](#-technologies-used)
- [Features](#-features)
- [Installation](#-installation)
- [A to Z Usage Guide](#-a-to-z-usage-guide)
- [Code Structure](#-code-structure)
- [Contributing](#-contributing)
- [License](#-license)
- [Credits](#-credits)

## 🎯 Project Overview

Cancer Survival Prediction Companion is a compassionate web application designed to assist healthcare providers and patients in understanding cancer survival predictions based on clinical parameters. The tool combines machine learning predictions with empathetic guidance, focusing on improving quality of life and informed decision-making.

### Mission Statement
To provide accurate, compassionate cancer survival predictions while maintaining human dignity and supporting informed healthcare decisions.

### Key Objectives
- Deliver clinically relevant survival predictions
- Provide compassionate, supportive guidance
- Empower patients and families with knowledge
- Support healthcare providers in patient communication
- Maintain ethical standards in medical AI applications

## 🔍 How It Works

The application uses a Random Forest machine learning model trained on comprehensive cancer patient data to predict 5-year survival outcomes based on:

### Input Parameters
1. **Age**: Patient's age at diagnosis
2. **Gender**: Male/Female
3. **BMI**: Body Mass Index
4. **Smoking Status**: Never/Former/Current
5. **Alcohol Consumption**: None/Low/Moderate/High
6. **Cancer Type**: Lung/Breast/Colorectal/Prostate/Stomach
7. **Cancer Stage**: Stage I/II/III/IV
8. **Treatment Type**: Surgery/Chemotherapy/Radiation/Immunotherapy/Combination
9. **Genetic Markers**: Mutation A/B/C/D/E
10. **Comorbidities**: Number of additional conditions
11. **Treatment Response**: Poor/Moderate/Good
12. **Follow-up Frequency**: Monthly/Quarterly/Biannual/Annual

### Prediction Process
1. **Data Input**: Healthcare provider enters patient parameters
2. **Preprocessing**: Input validation and formatting
3. **ML Inference**: Random Forest model processes data
4. **Result Interpretation**: Binary outcome (0: Not Surviving, 1: Surviving)
5. **Guidance Generation**: Compassionate recommendations and resources

## 🛠️ Technologies Used

### Frontend
- **HTML5**: Semantic structure
- **CSS3**: Modern styling with gradients and animations
- **JavaScript (ES6+)**: Interactive functionality

### Backend
- **Python 3.8+**: Core logic
- **Flask 2.0+**: Web framework
- **scikit-learn**: Machine learning (Random Forest)
- **NumPy & Pandas**: Data processing

### Model
- **Algorithm**: Random Forest Classifier
- **Training Data**: Synthetic cancer patient dataset
- **Features**: 12 clinical parameters
- **Output**: Binary survival prediction

### Development
- **VS Code**: IDE
- **Git/GitHub**: Version control
- **pip**: Package management

## ✨ Features

### Core Functionality
- 🎯 **ML-Powered Predictions**: Random Forest model for survival analysis
- 📊 **12-Parameter Input**: Comprehensive patient assessment
- 💡 **Compassionate Guidance**: Supportive recommendations based on outcomes
- 📱 **Responsive Design**: Mobile-first, works on all devices
- ♿ **Accessibility**: WCAG 2.1 compliant (keyboard navigation, ARIA labels)

### User Experience
- Clean, intuitive interface
- Clear form validation
- Empathetic language and tone
- Resource recommendations
- Privacy-focused design

### Technical Features
- RESTful API architecture
- Real-time predictions
- Error handling and validation
- Secure data processing
- Model persistence (joblib)

## 📥 Installation

### Prerequisites
```bash
Python 3.8 or higher
pip (Python package installer)
Git (for cloning)
```

### Step 1: Clone Repository
```bash
git clone https://github.com/Gururaj-GJ/Cancer-Survival-Prediction-Companion.git
cd Cancer-Survival-Prediction-Companion
```

### Step 2: Create Virtual Environment (Recommended)
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 4: Verify Installation
```bash
python --version  # Should be 3.8+
pip list  # Check installed packages
```

### Step 5: Run Application
```bash
python app.py
```

Access at: `http://127.0.0.1:5000`

### Troubleshooting
- **Port conflict**: Modify `app.py` port if 5000 is in use
- **Missing packages**: Run `pip install -r requirements.txt` again
- **Python version**: Ensure Python 3.8+
- **Model file**: Ensure `cancer_survival_model.pkl` exists

## 📖 A to Z Usage Guide

### For Healthcare Providers

#### Step 1: Access Application
- Open browser: `http://127.0.0.1:5000`
- Review disclaimer and ethical guidelines

#### Step 2: Input Patient Data
Fill all required fields:
1. **Patient Demographics**
   - Age (years)
   - Gender (Male/Female)

2. **Health Metrics**
   - BMI (Body Mass Index)
   - Smoking Status
   - Alcohol Consumption

3. **Clinical Information**
   - Cancer Type
   - Cancer Stage (I-IV)
   - Treatment Type
   - Genetic Markers

4. **Treatment Details**
   - Number of Comorbidities
   - Treatment Response
   - Follow-up Frequency

#### Step 3: Submit & Review Prediction
- Click "Predict Survival"
- Review binary outcome:
  - **Surviving**: Green indicator with supportive guidance
  - **Not Surviving**: Compassionate messaging with palliative care resources

#### Step 4: Patient Communication
- Use results as discussion starting point
- Provide context and support
- Share resources and guidance
- Encourage questions and concerns

### For Patients & Families

#### Understanding Results
- **Statistical Nature**: Predictions are estimates, not certainties
- **Individual Variation**: Your journey is unique
- **Professional Guidance**: Always consult your healthcare team

#### Using Resources
- Review recommended support services
- Explore quality of life guidance
- Connect with family resources
- Ask questions to your medical team

### Form Validation
- All fields are required
- Age: 0-120 years
- BMI: 10-60 range
- Comorbidities: 0-10 count
- Real-time error messages

### Privacy & Security
- No data storage
- No personal information collected
- Session-based processing only
- HIPAA-aware design principles

## 📸 Screenshots

![Main Interface - Mobile View](assets/images/Mobile-View-1.jpg)
*Mobile-responsive interface for easy data input on any device*

![Input Form - Mobile View](assets/images/Mobile-View-2.jpg)
*Comprehensive input form for patient assessment parameters*

![Results Display - Mobile View](assets/images/Mobile-View-3.jpg)
*Survival prediction results with compassionate guidance*

![Care Resources - Mobile View](assets/images/Mobile-View-4.jpg)
*Detailed care recommendations and quality of life considerations*

![Support Information - Mobile View](assets/images/Mobile-View-5.jpg)
*Additional support information and family guidance resources*

![Desktop view: Homepage and main interface](assets/images/Laptop-View-1.jpg)
*Laptop-View-1.jpg – Desktop view: Homepage and main interface*

![Desktop view: Clinical input form](assets/images/Laptop-View-2.jpg)
*Laptop-View-2.jpg – Desktop view: Clinical input form*

![Desktop view: Survival and time window guidance results](assets/images/Laptop-View-3.jpg)
*Laptop-View-3.jpg – Desktop view: Survival and time window guidance results*

![Desktop view: Comfort, care, and support resources](assets/images/Laptop-View-4.jpg)
*Laptop-View-4.jpg – Desktop view: Comfort, care, and support resources*

## 📁 Code Structure

```
Cancer-Survival-Prediction-Companion/
│
├── app.py                          # Flask application entry point
├── cancer_survival_model.pkl       # Trained Random Forest model
├── requirements.txt                # Python dependencies
├── README.md                       # This file
│
├── templates/
│   ├── index.html                 # Main application page
│   └── result.html                # Prediction results page
│
├── static/
│   ├── styles.css                 # Application styling
│   └── script.js                  # Client-side logic
│
└── assets/
    └── images/                    # Screenshot assets
```

### Key Files

#### `app.py`
- Flask routes and logic
- Model loading and prediction
- Input validation
- Response formatting

#### `templates/index.html`
- Input form
- Form validation
- Accessibility features
- Responsive design

#### `templates/result.html`
- Results display
- Conditional guidance
- Resource links
- Support information

#### `static/styles.css`
- Modern gradient design
- Responsive layouts
- Accessibility styling
- Animation effects

#### `static/script.js`
- Form validation
- AJAX submission (if implemented)
- Interactive elements
- Error handling

## 🤝 Contributing

### Ways to Contribute
1. **Report Bugs**: Open issues for any problems
2. **Suggest Features**: Propose compassionate enhancements
3. **Improve Documentation**: Clarify instructions
4. **Enhance Accessibility**: Improve WCAG compliance
5. **Add Resources**: Suggest patient support links

### Contribution Process
1. **Fork the Repository**
2. **Create Feature Branch**: `git checkout -b feature/YourFeature`
3. **Commit Changes**: `git commit -m 'Add compassionate feature'`
4. **Push to Branch**: `git push origin feature/YourFeature`
5. **Test Thoroughly**: Ensure no regressions
6. **Open a Pull Request**

### Contribution Guidelines
- Maintain compassionate, supportive language
- Ensure accessibility compliance
- Test on multiple devices/browsers
- Document all changes
- Respect patient privacy and dignity

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

### Usage Terms
- ✅ Free for educational purposes
- ✅ Free for healthcare research
- ⚠️ Not FDA approved for clinical use
- ⚠️ Requires professional medical oversight
- ❌ Not a substitute for professional medical advice

## 🙏 Credits

### Development
- **Created by**: Gururaj GJ
- **Purpose**: Educational demonstration of ML in healthcare
- **Inspiration**: Improving patient care through technology

### Acknowledgments
- scikit-learn community for ML frameworks
- Healthcare professionals for domain expertise
- Patients and families who inspire compassionate care

### Disclaimer

⚠️ **Important Medical Disclaimer**

This tool is for **educational and informational purposes only**. It is NOT:
- A replacement for professional medical advice
- FDA approved or clinically validated
- Suitable for making treatment decisions
- Guaranteed to be accurate for any individual

**Always consult qualified healthcare professionals** for:
- Diagnosis and treatment planning
- Medical decision-making
- Cancer care management
- Palliative care decisions

The predictions provided are statistical estimates based on historical data and may not reflect individual outcomes. Every patient's journey is unique.

---

**Remember**: Behind every data point is a human being with hopes, fears, and loved ones. This tool aims to serve with compassion, accuracy, and respect for human dignity.

For questions, feedback, or collaboration: [Your Contact Information]

*Last Updated: October 2025*
