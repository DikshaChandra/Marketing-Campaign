# Marketing Campaign Analysis with Pandas

- Conversion Rates
- Retention Rates
- Segmentation
- Data Visualization
- Attribution
- A/B Testing
## Description

With marketing campaign data from a hypothetical online subscription business, used Python and Pandas to translate common business questions into measurable outcomes. Looked into how the campaign performed, which channel(s) referred the most subscribers and dissected why a particular channel was underperforming.

- Assess contents and quality of data set
- Use feature engineering to create new columns
- Create functions to automate analysis (retention, conversion, segmentation)
- Segment users and visualize results to see group differences
- Identify issue in campaign and find cause
- Analyze an A/B test determining statistical significance with lifts and t-tests to see impact
## Python Libraries
- pandas
- numpy
- matplotlib
- scipy
## Challenges
The largest concern I had was when the overall marketing campaign retention rate came back as ~680% which could not be correct. From this point, I had double-checked my code and equations which were all correct. I used value_counts(), min(), max() and various tinkering to assess what was happening to the bool data type for the true/false values of 'is_retained'. I reloaded the data set and tested this before and after, only to discover and correct that converting the column from an object to bool was incorrectly converting missing values to true and false values. The issue was solved with fillna(False).
