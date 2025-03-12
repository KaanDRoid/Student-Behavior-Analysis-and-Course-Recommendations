# Student-Behavior-Analysis-and-Course-Recommendations
Analyzes student behavior and engagement in online learning, with a rule based and machine learning enhanced course recommendation system.

## Overview
This project analyzes student data from the Personalized Learning Dataset to uncover insights into student behavior, performance, and engagement in an online learning platform. By leveraging data analysis and visualization techniques, the project aims to identify key patterns in student demographics, course popularity, engagement levels, and dropout likelihood. Additionally, a simple rule-based course recommendation system is developed to provide personalized learning suggestions, enhancing the overall student experience and supporting educators in optimizing learning strategies.

## Steps
### Data Exploration and Cleaning
- Required Libraries: `import pandas as pd`
- Loaded the dataset and inspected its structure.
- Checked for missing values (none found) and ensured data consistency.

### Demographic Analysis
- Required Libraries: `import matplotlib.pyplot as plt`, `import seaborn as sns`
- Analyzed the distribution of students by age, gender, and education level to understand the platform's user base.
- Visualized age distribution, gender breakdown, and education levels using histograms, pie charts, and bar plots.

### Course Popularity and Feedback Analysis
- Required Libraries: `import matplotlib.pyplot as plt`, `import seaborn as sns`
- Identified the most popular courses based on enrollment numbers.
- Evaluated student satisfaction through average feedback scores per course using bar plots.

### Engagement and Performance Analysis
- Required Libraries: `import matplotlib.pyplot as plt`, `import seaborn as sns`
- Examined engagement levels (Low, Medium, High) and their impact on performance metrics (quiz scores, assignment completion rates, and final exam scores).
- Visualized engagement distribution and performance trends using pie charts and grouped bar plots.

### Dropout Likelihood Analysis
- Required Libraries: `import matplotlib.pyplot as plt`, `import seaborn as sns`
- Analyzed dropout likelihood across demographic groups, courses, and engagement levels.
- Visualized dropout rates and correlations with interaction metrics (e.g., time spent on videos, forum participation).

### Advanced Visualizations and Insights
- Required Libraries: `import matplotlib.pyplot as plt`, `import plotly.express as px`, `from dash import Dash, dcc, html, Input, Output`
- Created additional visualizations (e.g., hexmaps, scatter plots) to explore relationships between student interactions, performance, and demographics.
- Summarized key findings to support data-driven decision-making for educators.

## Tools Used
- Python (Pandas, NumPy)
- Data Visualization (Matplotlib, Seaborn, Plotly)
- Interactive Dashboard (Dash)
- Jupyter Notebook

## How to Run
Clone this repository and open the Jupyter Notebook:
```bash
git clone https://github.com/KaanDRoid/Student-Behavior-Analysis-and-Course-Recommendations.git
cd Student-Behavior-Analysis-and-Course-Recommendations
