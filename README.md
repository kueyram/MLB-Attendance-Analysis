# MLB Attendance Analysis

This project analyzes the attendance of the Los Angeles Dodgers during the 2022 MLB season. It aims to identify patterns and factors influencing game attendance using data visualization and linear regression modeling.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Correlation Analysis](#correlation-analysis)
- [Modeling](#modeling)
- [Conclusion](#conclusion)
- [How to Download the Project](#how-to-download-the-project)
- [Requirements](#requirements)
- [License](#license)

## Overview

The analysis focuses on understanding how different factors affect the attendance at Dodgers games. The project involves data cleaning, exploratory data analysis (EDA), correlation analysis, and predictive modeling using linear regression.

## Dataset

The dataset used for this project can be found [here](https://raw.githubusercontent.com/kueyram/MLB-Attendance-Analysis/refs/heads/main/data/dodgers-2022.csv). It contains the following columns:

- `month`: Month of the game
- `day`: Day of the month
- `day_of_week`: Day of the week
- `day_night`: Day or night game
- `opponent`: Opposing team
- `attend`: Attendance at the game
- `cap`: Cap promotion
- `shirt`: Shirt promotion
- `fireworks`: Fireworks night
- `bobblehead`: Bobblehead night
- `temp`: Temperature on game day

## Exploratory Data Analysis

1. **Attendance by Month**: A box plot shows attendance peaks in June and July, averaging around 50,000 fans, while other months have lower averages.
  
2. **Attendance Histogram**: A histogram indicates that attendance follows a normal distribution with an average around 40,000 attendees per game.
  
3. **Attendance by Day of the Week**: Attendance analysis reveals that Tuesdays have the highest and most consistent attendance, with a median around 50,000.
  
4. **Opponent Analysis**: Attendance varies significantly based on the opponent, with teams from larger cities drawing larger crowds.

5. **Promotional Events**: Analysis shows high attendance during bobblehead promotions, indicating that promotional events can significantly influence attendance.

## Correlation Analysis

A correlation matrix was created to examine the relationships between different numerical variables and attendance. Key findings include:
- A weak positive correlation (0.099) between attendance and temperature.
- A very weak correlation (0.027) between attendance and the day of the month.

## Modeling

A linear regression model was developed to predict attendance based on several features, including:
- Month
- Day
- Day of the week
- Day/Night games
- Various promotional events

## Key results include:
- The model explains approximately 18.32% of the variance in attendance (R-squared = 0.1832).
- Bobblehead promotions have a significant positive impact on attendance.

## Conclusion

The analysis highlights that Tuesdays and summer months (June and July) attract the most fans. Recommendations for increasing attendance include planning more promotions during slower months and capitalizing on busier times with special offers.

## How to Download the Project

To download the project, you can clone the GitHub repository using the following command:

```bash
git clone https://github.com/kueyram/MLB-Attendance-Analysis.git
```

## Requirements

To run this project, you will need the following libraries:

    pandas
    numpy
    matplotlib
    seaborn
    scikit-learn

You can install these libraries using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## License

This project is licensed under the MIT License. See the LICENSE file for more details.