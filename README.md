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
- **JavaScript (ES6+)**: Dynamic interactions and predictions

### Machine Learning
- **scikit-learn**: Random Forest Classifier
- **pandas**: Data manipulation
- **numpy**: Numerical computations

### Design Features
- Responsive design for mobile and desktop
- Accessibility-focused UI elements
- Color-coded feedback (green for positive, red for concerning)
- Smooth animations and transitions

## ✨ Features
### Core Functionality
- ✅ Real-time survival prediction
- ✅ Comprehensive patient parameter input
- ✅ Mobile-responsive design
- ✅ Compassionate result messaging
- ✅ Quality of life guidance
- ✅ Resource recommendations

### User Experience
- Clean, intuitive interface
- Clear form validation
- Immediate feedback
- Supportive language throughout
- Easy-to-understand results

### Ethical Considerations
- Transparent limitations disclosure
- Emphasis on professional consultation
- Compassionate communication
- Privacy-conscious design
- No data storage or tracking

## 📦 Installation
### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No server required for basic usage
- Python 3.7+ (for model training/updates)

### Quick Start
1. **Clone the repository**
   ```bash
   git clone https://github.com/Gururaj-GJ/Cancer-Survival-Prediction-Companion.git
   cd Cancer-Survival-Prediction-Companion
   ```

2. **Open the application**
   - Simply open `index.html` in your web browser
   - No build process required

3. **Start using**
   - Fill in the patient parameters
   - Click "Predict Survival" button
   - Review results and recommendations

### For Development
1. **Install Python dependencies** (if modifying ML model)
   ```bash
   pip install scikit-learn pandas numpy
   ```

2. **Model training** (optional)
   ```python
   # Train new model with updated data
   python train_model.py
   ```

## 📖 A to Z Usage Guide
### Step 1: Access the Application
- Open `index.html` in your browser
- Ensure JavaScript is enabled

### Step 2: Enter Patient Information
#### Basic Information
- **Age**: Enter numerical age (1-120)
- **Gender**: Select from dropdown
- **BMI**: Enter Body Mass Index (10-50)

#### Lifestyle Factors
- **Smoking Status**: Select appropriate category
- **Alcohol Consumption**: Select consumption level

#### Medical Information
- **Cancer Type**: Choose primary cancer type
- **Cancer Stage**: Select disease progression stage
- **Treatment Type**: Specify current treatment approach

#### Clinical Markers
- **Genetic Markers**: Select relevant genetic mutation
- **Comorbidities**: Number of additional health conditions (0-10)
- **Treatment Response**: Current response to treatment
- **Follow-up Frequency**: Scheduled follow-up intervals

### Step 3: Submit for Prediction
- Review all entered information
- Click "Predict Survival" button
- Wait for results (instant)

### Step 4: Interpret Results
#### If Prediction = Surviving (1)
- Green confirmation message
- Positive outlook guidance
- Quality of life recommendations
- Ongoing care suggestions

#### If Prediction = Not Surviving (0)
- Compassionate messaging
- Palliative care information
- Quality time recommendations
- Support resources

### Step 5: Take Action
- Discuss results with healthcare team
- Consider recommended resources
- Plan next steps in care journey
- Seek additional support as needed

## 🏗️ Code Structure
### File Organization
```
Cancer-Survival-Prediction-Companion/
│
├── index.html              # Main application file
├── README.md               # Documentation
├── assets/
│   └── images/            # Screenshot images
│       ├── Mobile-View-1.jpg
│       ├── Mobile-View-2.jpg
│       ├── Mobile-View-3.jpg
│       ├── Mobile-View-4.jpg
│       └── Mobile-View-5.jpg
└── (additional files as needed)
```

### Key Components
#### HTML Structure
- Semantic HTML5 elements
- Form inputs for all parameters
- Results display section
- Responsive container layout

#### CSS Styling
- CSS Grid and Flexbox layouts
- Custom color scheme (purple/blue gradient)
- Mobile-first responsive design
- Smooth transitions and animations

#### JavaScript Logic
- `predictSurvival()`: Main prediction function
- Input validation
- ML model weights embedded
- Result display logic
- Compassionate messaging system

### Machine Learning Model
- **Algorithm**: Random Forest Classifier
- **Features**: 12 input parameters
- **Output**: Binary classification (0/1)
- **Accuracy**: ~75% (model-dependent)

## 📸 Screenshots

![Main Interface - Mobile View](assets/images/Mobile-View-1.jpg)
*Mobile-responsive interface for easy data input on any device*

![Input Form](assets/images/Mobile-View-2.jpg)
*Comprehensive input form for patient assessment parameters*

![Results Display 1](assets/images/Mobile-View-3.jpg)
*Survival prediction results with compassionate guidance*

![Results Display 2](assets/images/Mobile-View-4.jpg)
*Detailed care recommendations and quality of life considerations*

![Results Display 3](assets/images/Mobile-View-5.jpg)
*Additional support information and family guidance resources*

## 🤝 Contributing
We welcome contributions that improve prediction accuracy, user experience, or compassionate communication.

### How to Contribute
1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/YourFeatureName
   ```
3. **Make your changes**
   - Follow existing code style
   - Test thoroughly
   - Update documentation
4. **Commit your changes**
   ```bash
   git commit -m "Add: Description of your changes"
   ```
5. **Push to your fork**
   ```bash
   git push origin feature/YourFeatureName
   ```
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
