# Relationships-Among-Physical-Activity-Stress-Levels-and-BMI-Categories
This study explores the relationships among physical activity, stress levels, and BMI categories in 374 respondents using correlation tests and data visualizations to identify patterns and associations without implying causation.

# Exploring the Relationships Among Physical Activity, Stress Levels, and BMI Categories

This study explores the relationships among physical activity, stress levels, and BMI categories in 374 respondents using correlation tests and data visualizations.

## Objectives
- Examine the relationship between physical activity and stress.
- Analyze how physical activity and stress relate to BMI categories.

## Dataset
The Sleep Health and Lifestyle dataset contains 374 observations and 13 variables. This analysis focuses on:
- Physical Activity Level
- Stress Level
- BMI Category

During preprocessing, "Normal Weight" was combined with "Normal" to standardize BMI labels.

## Methods
- Data cleaning and descriptive statistics
- Kendall’s correlation: physical activity vs stress
- Spearman’s correlation: physical activity vs BMI and stress vs BMI
- Significance level: 0.05

## Visualizations
- Boxplots of stress and physical activity by BMI category
- Scatter plot of physical activity vs stress
- Bar chart of respondent counts by BMI category
- Bubble plot of physical activity vs stress, grouped by BMI category

## Results
| Relationship | Coefficient | p-value |
|---|---:|---:|
| Physical Activity vs Stress (Kendall) | -0.0390 | 0.3333 |
| Physical Activity vs BMI (Spearman) | 0.0610 | 0.2393 |
| Stress vs BMI (Spearman) | 0.1397 | 0.0068 |

Stress showed a statistically significant but weak positive association with BMI category. The other two correlations were not statistically significant.

## Tools
R, R Markdown, ggplot2, plotly, dplyr, and knitr.

## How to Run
1. Download the R Markdown file and CSV dataset.
2. Place both files in the same folder.
3. Open the R Markdown file in RStudio.
4. Install the required packages:
   install.packages(c("rmarkdown", "ggplot2", "plotly", "dplyr", "knitr"))
5. Click Knit to generate the report.

## Limitations
BMI groups are unequal in size, with only 10 respondents in the Obese category. The analysis does not adjust for age, gender, or occupation. Reported p-values are unadjusted for multiple comparisons. Correlation does not establish causation.
