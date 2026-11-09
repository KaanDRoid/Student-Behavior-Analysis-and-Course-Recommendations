# Student Behavior Analysis and Course Recommendations

Exploratory analysis of student behavior on an online learning platform using the Personalized Learning Dataset. The notebook looks at who the students are, which courses they take, how engagement relates to performance and dropout, and then builds two small rule-based course recommenders. A minimal Dash dashboard is included at the end for filtering scores by engagement and education level.

## Data

`personalized_learning_dataset.csv` has 10,000 rows, one per student, with no missing values. Columns include age, gender, education level, course name, time spent on videos, quiz attempts and scores, forum participation, assignment completion rate, engagement level (Low/Medium/High), final exam score, learning style, feedback score (1-5) and dropout likelihood (Yes/No).

## What the notebook does

1. Loads the data and checks types and missing values.
2. Demographics: age histogram, gender pie chart, education level counts.
3. Courses: enrollment per course and average feedback score per course.
4. Engagement vs. performance: mean quiz score, assignment completion and final exam score per engagement level.
5. Dropout: dropout counts by gender, education and engagement level, and a correlation heatmap between interaction metrics and dropout.
6. Recommendations:
   - `recommend_course()` suggests a next course from the current course, final exam score (> 80) and engagement level.
   - `recommend_course_with_thresholds()` first puts students in performance tiers (High >= 85, Medium 65-84, Low < 65) and then picks a suggestion per tier and engagement level.
7. Extra plots (box plots, Plotly scatter, hexbin) and a Dash app with dropdown filters.

## Results

- Enrollment and average feedback (around 3 out of 5) are very similar across the five courses.
- Engagement level shows almost no difference in quiz scores, exam scores or dropout likelihood, so it is a weak signal in this dataset.
- Example output of the threshold recommender: S00001 -> Foundational Learning Skills, S00002 -> Advanced Python Programming, S00004 -> Introduction to Data Science.

## How to run

```bash
pip install -r requirements.txt
jupyter notebook personalized_learning.ipynb
```

The Dash app in the last code cell runs inline in Jupyter (Dash 2.11+).

## Repository layout

```
personalized_learning.ipynb        analysis notebook
personalized_learning_dataset.csv  dataset
requirements.txt
LICENSE
```
