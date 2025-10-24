# Cancer Survival Prediction Companion

🩺 **A compassionate tool for palliative care planning and survival prediction that works completely offline**

This tool helps healthcare providers and families make informed decisions during challenging times by providing data-driven insights while maintaining complete privacy and accessibility without internet connection.

---

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

---

## 🎯 Project Overview

### Purpose
The Cancer Survival Prediction Companion is designed specifically for palliative care planning, helping healthcare providers and families understand potential outcomes and plan appropriate care strategies. The tool emphasizes:

- **Compassionate Care**: Designed with sensitivity for end-of-life planning
- **Privacy First**: Works completely offline - no data leaves your device
- **Accessibility**: Simple interface that works without technical expertise
- **Evidence-Based**: Uses validated clinical parameters for predictions

### Key Benefits
- 🔒 **Complete Privacy**: No internet connection required, all data stays local
- 📱 **Universal Access**: Works on any device with a web browser
- 🏥 **Clinical Validation**: Based on established palliative care indicators
- 💝 **Compassionate Design**: Sensitive language and supportive guidance

---

## 🔄 How It Works

### Step-by-Step Process

1. **Data Input**: Clinicians or caregivers input patient symptoms and clinical parameters
2. **Assessment**: The tool evaluates multiple palliative care indicators:
   - Respiratory function (breathlessness levels)
   - Nutritional status (food intake, swallowing ability)
   - Digestive function (nausea, bowel movements)
   - Pain levels and bone involvement
   - Advanced imaging data (optional)

3. **Calculation**: Uses weighted algorithms based on palliative care research
4. **Results**: Provides compassionate guidance with:
   - Survival probability ranges
   - Care recommendations
   - Quality of life considerations
   - Family support suggestions

### Offline Features
- **Self-contained**: All logic runs in the browser
- **No data transmission**: No servers, APIs, or external connections
- **Instant results**: No waiting for network requests
- **Portable**: Can be saved and used on any device

---

## 💻 Technologies Used

### Frontend Technologies
- **HTML5**: Semantic markup for accessibility
- **CSS3**: Modern styling with responsive design
- **Vanilla JavaScript**: Pure JS for maximum compatibility
- **Web APIs**: Local storage, form validation

### Key Libraries & Frameworks
- **No external dependencies**: Completely self-contained
- **Progressive Web App (PWA) ready**: Can be installed offline
- **Bootstrap-like CSS**: Custom responsive grid system

### Development Tools
- **Version Control**: Git
- **Testing**: Manual testing across browsers
- **Validation**: HTML5 form validation

---

## ✨ Features

### Clinical Assessment Parameters
- **Breathlessness Scale**: 5-point clinical scale (0-4)
- **Respiratory Distress**: Speaking difficulty indicator
- **Cough Frequency**: Daily episode tracking
- **Gastrointestinal**: Nausea/vomiting episodes
- **Nutritional Status**: Days without solid food
- **Medication Tolerance**: Swallowing ability
- **Bowel Function**: Constipation tracking
- **Renal Function**: Urine output monitoring (optional)
- **Pain Assessment**: 0-10 pain scale
- **Metastasis Indicators**: Bone involvement
- **Advanced Imaging**: PET scan SUV values (optional)

### User Interface Features
- **Intuitive Design**: Clean, medical-grade interface
- **Form Validation**: Real-time input validation
- **Responsive Layout**: Works on desktop, tablet, mobile
- **Accessibility**: Screen reader compatible
- **Clear Results**: Easy-to-understand output

### Privacy & Offline Features
- **No Data Collection**: Zero telemetry or tracking
- **Local Processing**: All calculations done client-side
- **No Registration**: No accounts or personal data required
- **Portable**: Single HTML file that can be shared
- **Version Control**: Can be saved with patient data locally

---

## 🚀 Installation

### Method 1: Direct Download
1. Download the `index.html` file from this repository
2. Save it to your local computer/device
3. Double-click to open in any web browser
4. Tool is ready to use offline!

### Method 2: Clone Repository
```bash
git clone https://github.com/Gururaj-GJ/Cancer-Survival-Prediction-Companion.git
cd Cancer-Survival-Prediction-Companion
# Open index.html in your preferred browser
```

### Method 3: Web Server (Optional)
```bash
# If you prefer running on a local server:
python -m http.server 8000
# Or
npx serve .
# Then visit http://localhost:8000
```

### System Requirements
- **Browser**: Any modern web browser (Chrome, Firefox, Safari, Edge)
- **Internet**: Not required after download
- **Storage**: <1MB disk space
- **Platform**: Windows, Mac, Linux, mobile devices

---

## 📖 A to Z Usage Guide

### Getting Started
1. **Open the Tool**: Launch `index.html` in your browser
2. **Review Interface**: Familiarize yourself with input fields
3. **Gather Information**: Collect patient clinical data

### Input Parameters Guide

#### Basic Respiratory Assessment
- **Breathlessness Level**: Select from dropdown (0-4 scale)
  - 0: No breathlessness
  - 1: Only on exertion
  - 2: Walking on level ground
  - 3: After just a few steps
  - 4: Even at rest
- **Speaking Difficulty**: Check if patient gets breathless when talking

#### Symptom Tracking
- **Cough Episodes**: Enter number per day (0-100)
- **Vomiting Episodes**: Enter number per day (0-20)
- **Days Without Food**: Enter days without solid food (0-30)
- **Medication Tolerance**: Check if can swallow pills/liquids
- **Bowel Movement**: Enter days without bowel movement (0-21)

#### Optional Advanced Parameters
- **Urine Output**: 24-hour volume in ml (optional)
- **Pain Level**: Use slider (0-10 scale)
- **Bone Metastasis**: Check if doctor mentioned bone spread
- **PET SUV Value**: Enter bone SUV max if available

### Reading Results
- **Survival Estimates**: Probability ranges with confidence intervals
- **Care Recommendations**: Specific palliative care suggestions
- **Quality Measures**: Comfort and symptom management advice
- **Family Guidance**: Support recommendations for caregivers

### Best Practices
- ✅ Use most recent clinical data
- ✅ Involve healthcare team in interpretation
- ✅ Consider results as guidance, not absolute predictions
- ✅ Update assessments regularly as condition changes
- ❌ Don't use as sole basis for major medical decisions
- ❌ Don't share results without proper clinical context

### Screenshot Placeholders
```
[Main Interface Screenshot]
[Input Form Screenshot]
[Results Display Screenshot]
[Mobile View Screenshot]
```

---

## 📁 Code Structure

### Main Files
```
Cancer-Survival-Prediction-Companion/
├── index.html              # Main application file
├── README.md              # This documentation
├── assets/                # Static assets (if any)
│   ├── css/              # Stylesheets
│   ├── js/               # JavaScript modules
│   └── images/           # Icons, logos
├── docs/                 # Additional documentation
└── tests/                # Testing files
```

### Key Components

#### `index.html`
- **Main Structure**: Contains all HTML, CSS, and JavaScript
- **Form Handling**: Input validation and data collection
- **Calculation Engine**: Survival prediction algorithms
- **Results Display**: Output formatting and presentation

#### JavaScript Modules (within index.html)
- **`calculateSurvival()`**: Main prediction algorithm
- **`validateInput()`**: Form validation functions
- **`displayResults()`**: Results formatting and display
- **`resetForm()`**: Form reset functionality

#### CSS Sections
- **Layout Styles**: Responsive grid and containers
- **Form Styles**: Input field styling and validation states
- **Results Styles**: Output formatting and typography
- **Mobile Styles**: Responsive breakpoints

#### Calculation Logic
- **Weighted Scoring**: Each parameter has clinical weight
- **Risk Stratification**: Multiple risk categories
- **Confidence Intervals**: Uncertainty quantification
- **Validation Bounds**: Input range checking

---

## 🤝 Contributing

### How to Contribute
1. **Fork the Repository**: Click the Fork button on GitHub
2. **Create a Branch**: `git checkout -b feature/your-feature-name`
3. **Make Changes**: Implement your improvements
4. **Test Thoroughly**: Ensure functionality across browsers
5. **Submit Pull Request**: Describe your changes clearly

### Contribution Guidelines
- **Code Quality**: Follow existing coding patterns
- **Documentation**: Update README for any new features
- **Testing**: Test on multiple browsers and devices
- **Privacy**: Maintain offline-first approach
- **Sensitivity**: Maintain compassionate language and approach

### Areas for Contribution
- 🌐 **Internationalization**: Multiple language support
- 📱 **Mobile UX**: Enhanced mobile experience
- ♿ **Accessibility**: Screen reader improvements
- 📊 **Visualizations**: Charts and graphs for results
- 🔬 **Algorithm**: Evidence-based improvements to prediction model
- 📚 **Documentation**: User guides and clinical documentation

---

## 📄 License

### Open Source License
This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

### Permission Summary
- ✅ Commercial use
- ✅ Modification
- ✅ Distribution
- ✅ Private use
- ❗ No warranty or liability

### Medical Disclaimer
⚠️ **Important**: This tool is for informational purposes only and should not replace professional medical advice. Always consult with qualified healthcare providers for medical decisions.

---

## 🙏 Credits

### Development
- **Primary Developer**: [Gururaj-GJ](https://github.com/Gururaj-GJ)
- **Concept**: Palliative care prediction modeling

### Clinical Sources
- Palliative Performance Scale research
- WHO symptom assessment guidelines
- Oncology nursing assessment protocols
- Evidence-based palliative care literature

### Technical Acknowledgments
- HTML5 form validation standards
- Web accessibility guidelines (WCAG)
- Progressive Web App best practices
- Privacy-by-design principles

### Inspiration
- Healthcare professionals working in palliative care
- Families navigating difficult healthcare decisions
- Open-source healthcare technology community

---

## 📞 Support

For questions, suggestions, or support:
- **GitHub Issues**: [Report bugs or request features](https://github.com/Gururaj-GJ/Cancer-Survival-Prediction-Companion/issues)
- **Discussions**: [Community discussions](https://github.com/Gururaj-GJ/Cancer-Survival-Prediction-Companion/discussions)

---

*Built with ❤️ for compassionate healthcare*
