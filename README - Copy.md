# 🤖 AI Salary Predictor - Enterprise Edition

<!-- Badges -->

![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Regression-orange)
![UI](https://img.shields.io/badge/UI-Gradio-green)

## 📌 About The Project

An advanced machine learning system based on regression to analyze and price technical talents in the global market with high accuracy. This predictive analytics tool eliminates guesswork by leveraging historical data (experience, location, job title) to accurately forecast AI industry salaries.

**Primary KPI:** Achieve an R² Score exceeding 80% to ensure reliable results for production environments.

## 📊 Dataset & Analytics

The models were trained on a massive global database covering markets in America, Europe, and Asia[cite: 3].

- **Initial Records:** 15,000+[cite: 3].
- **Balanced Records:** 27,738 (achieved via Up-Sampling techniques)[cite: 3].
- **Features:** 18 independent features[cite: 3].
- **Insights:** Discovered a strong positive correlation (0.74) between years of experience and income level, and uncovered the "Job Title Ceiling" paradox which proved that tree-based algorithms were strictly required[cite: 3].

## ⚙️ Data Engineering Pipeline

To prepare the raw data for AI training, we implemented a rigorous engineering pipeline:

1. **Clean & Drop:** Handled missing values and anomalies[cite: 3].
2. **Encoding:** Applied categorical encoding to 84 columns[cite: 3].
3. **Up-Sampling:** Balanced the dataset, which was the key to preventing bias and improving model accuracy[cite: 3].
4. **Standard Scale:** Unified feature scaling across all variables[cite: 3].

## 🧠 Model Performance

We trained, tuned, and evaluated 6 regression algorithms in parallel[cite: 3]. The tree-based models significantly outperformed linear algorithms:

| Model                | R² Score            | Status                      |
| -------------------- | ------------------- | --------------------------- |
| 🏆 **Random Forest** | **96.76%**[cite: 3] | **Selected for Production** |
| 🏆 **XGBoost**       | **96.37%**[cite: 3] | Excellent                   |
| Polynomial (D2)      | 94.37%[cite: 3]     | Good                        |
| Linear Regression    | 89.48%[cite: 3]     | Baseline                    |
| KNN Regressor        | 82.92%[cite: 3]     | Baseline                    |
| AdaBoost             | 77.25%[cite: 3]     | Underperformed              |

## 🚀 Production & Deployment

We transformed the models into a fully functional software product:

- **Persistence:** The winning Random Forest model was serialized and saved as a `.joblib` file for rapid inference[cite: 3].
- **User Interface:** Developed a dynamic, real-time web UI using **Gradio**[cite: 3].
- **Real-time Engine:** Processes user inputs instantly to predict and display the expected salary in US Dollars[cite: 3].

## 💻 Getting Started

### Prerequisites

- Python 3.8 or higher
- pip package manager

### Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/ai-salary-predictor-ml.git](https://github.com/YOUR_USERNAME/ai-salary-predictor-ml.git)
   cd ai-salary-predictor-ml
   ```
