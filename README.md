# Influence of Daily Routine on Semester Marks

A statistical analysis examining the relationship between students' daily routines and their academic performance (semester marks) using multivariate regression modeling.

## 📋 Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Files Structure](#files-structure)
- [How to Run](#how-to-run)
- [Key Findings](#key-findings)
- [Author](#author)

## 📚 Project Overview

This dissertation analyzes how daily routine factors influence undergraduate semester marks. The study investigates whether daily habits like self-study duration, physical exercise, sleep, travel time, and media usage have a statistically significant relationship with academic performance.

**Institution:** St. Xavier's College (Autonomous), Kolkata  
**Department:** Statistics  
**Degree:** Statistics Honours (Undergraduate)  
**Supervisor:** Prof. Mausumi Bose

## 📊 Dataset

- **Sample Size:** 25 students
- **Population:** UG Semester 6 Statistics students (2025 batch)
- **Time Period:** Even Semester (January 2024 - June 2024)
- **Response Variable:** Semester 4 marks (percentage out of 500)

### Predictor Variables
1. **Self-Study (SS)** - Daily average percentage duration
2. **Physical Exercise (PE)** - Daily average percentage duration
3. **Sleep (SL)** - Daily average percentage duration
4. **Travel (TR)** - Daily average percentage duration
5. **Media-Usage (MU)** - Daily average percentage duration

## 🔬 Methodology

### Statistical Techniques Used
1. **Sample Survey** - For sample size selection
2. **Descriptive Analysis** - Mean, standard deviation, skewness, kurtosis
3. **Bivariate Analysis** - Individual predictor relationships
4. **Multivariate Analysis** - 6-variate linear regression model
5. **Cramer's Rule** - For coefficient estimation

### Key Model
**6-Variate Linear Regression Model:**
```
M = 53.12845 - (0.0433*SS) - (0.8802*PE) + (0.6197*SL) + (0.7585*TR) + (0.1120*MU)
```

Where M = Percentage marks (response variable)

## 📁 Files Structure

```
dissertation-repository/
├── README.md                          # This file
├── Dissertation_Sulagna_Roy.pdf       # Full dissertation document
├── Data/
│   ├── collected_data_set.csv         # Raw data from questionnaire
│   └── processed_data_set.csv         # Cleaned and processed data
├── R_Code/
│   ├── data_processing.R              # Data conversion & processing
│   ├── regression_analysis.R          # Multivariate regression
│   ├── descriptive_analysis.R         # Univariate analysis
│   └── visualization.R                # Histogram plots
└── Results/
    ├── Model_Summary.txt              # Regression coefficients
    └── Statistical_Summary.txt        # Descriptive statistics
```

## 🚀 How to Run

### Prerequisites
- R (version 3.6+)
- RStudio (recommended)
- Required packages: `Matrix` (for rank checking)

### Installation
1. Clone this repository
```bash
git clone https://github.com/yourusername/dissertation-daily-routine-marks.git
cd dissertation-daily-routine-marks
```

2. Open R or RStudio and set your working directory
```R
setwd("your/path/to/repository")
```

3. Run the analysis scripts in order
```R
# Step 1: Load and process data
source("R_Code/data_processing.R")

# Step 2: Perform descriptive analysis
source("R_Code/descriptive_analysis.R")

# Step 3: Run regression analysis
source("R_Code/regression_analysis.R")

# Step 4: Generate visualizations
source("R_Code/visualization.R")
```

## 📈 Key Findings

### Main Results

**6-Variate Model Interpretation:**
- **Self-Study:** Negative coefficient (-0.0433) → Excessive study time shows minimal impact
- **Physical Exercise:** Negative coefficient (-0.8802) → Less exercise correlates with slightly higher marks
- **Sleep:** Positive coefficient (+0.6197) → More sleep significantly improves marks (+37.18% per hour)
- **Travel:** Positive coefficient (+0.7585) → Travel time shows positive correlation (+45.51% per hour)
- **Media-Usage:** Positive coefficient (+0.1120) → Limited media usage beneficial (+6.72% per hour)

### Descriptive Statistics
- **Average Marks:** 73.99% (out of 100%)
- **Average Self-Study:** 2 hours 54 minutes per day
- **Average Sleep:** 7 hours 2 minutes per day
- **Average Physical Exercise:** 40 minutes 35 seconds per day

### Distribution Patterns
- All variables show **positive skewness** (larger number of students tend toward lower values)
- Marks distribution is **platykurtic** (flat, evenly spread)
- Sleep shows **leptokurtic** distribution (peaked, concentrated)

## 💡 Conclusions

1. **Sleep is Critical** - Adequate sleep significantly improves academic performance
2. **Quality Over Quantity** - Self-study duration alone doesn't guarantee better marks; quality matters
3. **Balanced Routine** - Students need balanced daily routines, not excessive study
4. **Physical Health** - Physical exercise and proper travel management contribute to success
5. **Digital Balance** - Moderate media usage is acceptable; complete avoidance unnecessary

## 📊 Visualizations

The repository includes 6 histogram plots showing the distribution of:
- Semester 4 marks
- Self-study duration
- Physical exercise duration
- Sleep duration
- Travel time
- Media usage

## 👩‍🎓 Author

**Sulagna Roy**  
Roll No: 2-14-22-0458  
Statistics Department  
St. Xavier's College (Autonomous), Kolkata

## 📝 License

This dissertation is submitted as partial fulfillment of Bachelor of Science (Statistics Honours) degree requirements at St. Xavier's College (Autonomous), Kolkata.

## 📧 Contact

For questions or clarifications about this research:
- Email: sulagna01royofficial@gmail.com
- GitHub: https://github.com/sulagna01royofficial
- LinkedIn: www.linkedin.com/in/sulagna01-roy
---

## 📚 References

The dissertation includes comprehensive citations from:
- Statistics and research methodology texts
- Academic publications on student performance
- Educational psychology resources

See the full dissertation PDF for complete references and detailed methodology.

---

**Last Updated:** April 2025  
**Dissertation Status:** Submitted & Accepted
