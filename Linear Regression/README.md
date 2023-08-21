## Linear Regression 📈

## Explanation of the Code:

The provided code performs a data analysis and visualization task using Python's libraries. Here's a detailed breakdown of each part of the code:

1. **Imports:**
   The code begins by importing necessary libraries, including `matplotlib.pyplot` for plotting, `numpy` for numerical operations, `pandas` for data handling, `scipy.stats` for statistical functions, and `random` for generating random numbers.

2. **Loading Data:**
   The `pd.read_excel` function is used to load data from an Excel file named 'Year7Data - 2023.xlsx' from the sheet named 'Sheet1' into a Pandas DataFrame named `df`.

3. **Printing Data:**
   The loaded DataFrame `df` is printed, displaying the data in the console.

4. **Extracting Data:**
   The relevant columns are extracted from the DataFrame `df`. `classes`, `grades`, `x1`, and `y` are defined to store information about class categories, letter grades, CT1 scores, and Total scores, respectively.

5. **Converting Letter Grades to Classes:**
   A loop iterates through each row in the dataset to convert letter grades ('A', 'B', 'C', 'D', and others) to numerical classes. These classes are then stored in the `classes` list, which will be used for color-coding in the plot.

6. **Linear Regression:**
   The code performs linear regression to find a linear relationship between the 'CT1' scores (`x1`) and the 'Total' scores (`y`). The `stats.linregress` function is used to calculate the slope, intercept, correlation coefficient (`r`), p-value (`p`), and standard error (`std_err`) of the regression line.

7. **Linear Function for Prediction:**
   The `myfunc` function is defined to represent the linear regression line. It takes an input `x` and returns the predicted `y` value based on the linear relationship determined by the regression.

8. **Predicting New Values:**
   The code generates a random new value for `x` within the range of the 'CT1' scores (`x1`). It calculates the corresponding predicted `y` value using the `myfunc` function and rounds it to an integer (`roundY`).

9. **Scatter Plot and Annotations:**
   A scatter plot is created using the 'CT1' scores (`x1`) as x-axis values and 'Total' scores (`y`) as y-axis values. The points are color-coded according to the numerical classes stored in the `classes` list. The new prediction point is also plotted in red and annotated with its coordinates.

10. **Plotting Linear Regression Line:**
   The linear regression line is plotted using `x1` as x-axis values and `mymodel` (predicted `y` values) as y-axis values.

11. **Labels, Title, and Grid:**
   Labels are added to the x and y axes, and a title is given to the plot. A grid is displayed to aid visualization.

12. **Saving and Displaying the Plot:**
   The plot is saved as an image named 'linearRegression.png', and then displayed using `plt.show()`.

## Explanation of the Dataset:

The dataset used in this code appears to contain information about student performance, specifically related to 'CT1' scores, 'CT2' scores, 'Port' scores, and 'Total' scores. Additionally, the dataset includes a column named 'I Grade' which represents letter grades associated with student performance.

## Explanation of Linear Regression:

Linear regression is a statistical technique used to model the relationship between two or more variables by fitting a linear equation to observed data. In the context of this code, linear regression is applied to establish a linear relationship between the 'CT1' scores and the 'Total' scores of students.

The linear regression process involves finding the best-fitting line (regression line) that minimizes the difference between the predicted values (based on the line) and the actual observed values (in this case, 'Total' scores). The line is defined by its slope and intercept, which are calculated using statistical methods. The goal is to make predictions based on the linear relationship found.

In the code, the `stats.linregress` function calculates these parameters, and the `myfunc` function represents the linear equation (`y = mx + b`) where `m` is the slope and `b` is the intercept. This equation can then be used to predict 'Total' scores (`y`) based on 'CT1' scores (`x1`).

By applying linear regression, we can analyze the correlation and predict values between variables, making it a powerful tool for various data analysis and prediction tasks.

### 📝 License

The code and documentation in this repository are licensed under the MIT License.
