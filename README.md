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

  <img width="729" height="481" alt="Screenshot 2026-09-21 at 18 09 05" src="https://github.com/user-attachments/assets/824ec58e-c271-4fa0-9a4b-3dbb99f8336b" />

The graph shows that individuals classified as Obese tend to have higher stress levels compared to those in other BMI categories. Statistical testing supports this observation, indicating a significant relationship between BMI Category and Stress Level. 


- Scatter plot of physical activity vs stress

<img width="744" height="467" alt="Screenshot 2026-09-21 at 18 15 31" src="https://github.com/user-attachments/assets/3f496d62-5abb-4e55-85d7-e54ff36ec6b5" />

This scatterplot illustrtes the relationship between Physical Activity Level and Stress Level. The data points appear widely dispersed, indicating no clear correlation between these two variables. This suggests that in this dataset, stress levels are not strongly associated with physical activity levels.


- Bar chart of respondent counts by BMI category
  <img width="744" height="421" alt="Screenshot 2026-09-21 at 18 16 05" src="https://github.com/user-attachments/assets/7a398be4-472d-4e02-9316-0c99a574ee46" />

The bar chart shows that 216 respondents belong to the Normal BMI category, followed by 148 in the Overweight category and 10 in the Obese category. These unequal group sizes should be considered when comparing patterns, as observations from the Obese group are based on a much smaller sample.

- Bubble plot of physical activity vs stress, grouped by BMI category
  <img width="651" height="403" alt="Screenshot 2026-09-21 at 18 16 34" src="https://github.com/user-attachments/assets/e617d950-9ecb-4171-a5e9-2af08af62e78" />

The bubble plot displays physical activity and stress levels within each BMI category, with larger bubbles representing more respondents at the same combination of values. The Normal and Overweight groups show varied patterns, with no consistent upward or downward trend. For example, the Overweight group includes clusters at activity level 75 with stress level 3 and activity level 90 with stress level 8. In the Obese group, higher activity levels visually correspond to lower stress levels, but this pattern is based on only 10 respondents and requires cautious interpretation. The plot alone does not establish statistical significance or causation.



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
