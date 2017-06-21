# Exploratory Data Analysis for Conversion Rate Dataset

We have data about users who hit our site: whether they converted or not as well as some of their characteristics such as their country, the marketing channel, their age, whether they are repeat users and the number of pages visited during that session (as a proxy for site activity/time spent on site).

**Goal:**
* Predict conversion rate
* Come up with recommendations for the product team and the marketing team to improve conversion rate


**Data:** Present under data/conversion_data.csv

**Table: "conversion_data" - information about signed-in users during one session. Each row is a user session.**

* country : user country based on the IP address
* age : user age. Self-reported at sign-in step
* new_user : whether the user created the account during this session or had already an account and simply came back to the site
* source : marketing channel source
    * Ads: came to the site by clicking on an advertisement
    * Seo: came to the site by clicking on search results
    * Direct: came to the site by directly typing the URL on the browser
* total_pages_visited: number of total pages visited during the session.
    * This is a proxy for time spent on site and engagement during the session.
* converted: this is our label. 1 means they converted within the session, 0 means they left without buying anything.
    * The company goal is to increase conversion rate: # conversions / total sessions.


**Question 1**

Function that returns a list of the names of categorical variables

* Define a function with name get_categorical_variables
* Pass dataframe as parameter (Read csv file and convert it into pandas dataframe)
* Return list of all categorical fields available.


**Question 2**

Function that returns the list of the names of numeric variables

* Define a function with name get_numerical_variables
* Pass dataframe as parameter (Read csv file and convert it into pandas dataframe)
* Return list of all numerical fields available.


**Question 3**

Function that returns, for numeric variables, mean, median, 25, 50, 75th percentile

* Define a function with name get_numerical_variables_percentile
* Pass dataframe as parameter (Read csv file and convert it into pandas dataframe)
* Return dataframe with following columns:
    * variable name
    * mean
    * median
    * 25th percentile
    * 50th percentile
    * 75th percentile


**Question 4**

For categorical variables, get modes

* Define a function with name get_categorical_variables_modes
* Pass dataframe as parameter (Read csv file and convert it into pandas dataframe)
* Return dict object with following keys:
    * converted
    * country
    * new_user
    * source


**Question 5**

For each column, list the count of missing values

* Define a function with name get_missing_values_count
* Pass dataframe as parameter (Read csv file and convert it into pandas dataframe)
* Return dataframe with following columns:
    * var_name
    * missing_value_count


**Question 6**

Plot histograms using different subplots of all the numerical values in a single plot

* Define a function with name plot_histogram_with_numerical_values
* Pass dataframe and list of columns you want to plot as parameter
* Plot the graph
* Add column names as plot names (In case you dont understand this please connect with instructor)
* Change the histogram colour to yellow
* Fit a normal curve on those histograms (In case you dont understand this please connect with instructor)


**Question 7**

Plot facet box plots to check out the distribution according to the target variable

* Define a function with name plot_facet_box
* Pass dataframe and list of columns you want to plot as parameter
* Plot the graph



