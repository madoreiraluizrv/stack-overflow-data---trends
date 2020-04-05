
### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3. However, if you need to know which libraries are used, here they are: numpy, pandas, matplotlib and collections.

## Project Motivation<a name="motivation"></a>

For this project, I was interestested in using Stack Overflow survey data from 2017-2019 to work on:

1. Business Understanding

I wanted to better understand and investigate the following questions:\n
a. What languages were most popular in each year?

2. Data Understanding

Here we used the StackOverflow survey data from the last three years to attempt to answer our questions of interest. We mostly used the data to help us arrive at our questions of interest.

In the process of understand the data, I also analyzed (just checking the CSV on Excel) the survey results from 2011-2016. Unfortunately, the survey didn't use the same questions at those years, so it was not possible to compare the results for some of the trend that I wanted to understand.

3. Prepare Data

From working with missing data to finding a way to work with categorical variables, passing by detailing multiple choice questions, I used many different processes to clean the data before using in the models and visualizations.

4. Model Data

For question 1, there was no need for machine learning, but I had to build a new dataframe with only language usage information and then model it to show me the ranking of each language in each year.

5. Results

Results are the findings from our wrangling and modeling. They are the answers you found to each of the questions. And for each of the answers, some kind of visualization (graphs) of the results was built.

6. Deploy

The deployment process was to create this github repository and then the medium post, describing the results, which you can find in the results section.

## File Descriptions <a name="files"></a>

There are x notebooks available here to showcase work related to the above questions.  Each of the notebooks is exploratory in searching through the data pertaining to the questions showcased by the notebook title.  Markdown cells were used to assist in walking through the thought process for individual steps.

1. LanguageRanking.ipynb
Notebook that solve question 'a' and shows a final graph with the ranking evolution of each language between 2017 and 2019.

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](), but here is a summary:
a. The three most used languages continued to be Java, Javascript and C, but C came ahead of the other two since 2018, and Objective C dropped many positions since 2017 (Swift becoming the go-to language on iOS development could be the reason, even though Swift ranking also decreased during the same time).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Must give credit to Stack Overflow for the data.  You can find more information at the link available [here](https://insights.stackoverflow.com/survey).  Otherwise, feel free to use the code here as you would like! And you have any feedback, please share

