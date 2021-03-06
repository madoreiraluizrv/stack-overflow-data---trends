
### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3. However, if you need to know which libraries are used, here they are: numpy, pandas, matplotlib, collections, sklearn, signal and contextlib.

## Project Motivation<a name="motivation"></a>

For this project, I was interestested in using Stack Overflow survey data from 2017-2019 to work on:

1. Business Understanding

I wanted to better understand and investigate the following questions:

a. What languages were most popular in each year?

b. What platforms were the most desired in each year?

c. Did the most important variables to predict salaries changed?

2. Data Understanding

Here we used the StackOverflow survey data from the last three years to attempt to answer our questions of interest. We mostly used the data to help us arrive at our questions of interest.

In the process of understand the data, I also analyzed (just checking the CSV on Excel) the survey results from 2011-2016. Unfortunately, the survey didn't use the same questions at those years, so it was not possible to compare the results for some of the trend that I wanted to understand.

3. Prepare Data

From working with missing data to finding a way to work with categorical variables, passing by detailing multiple choice questions, I used many different processes to clean the data before using in the models and visualizations.

Specifically on the coefficients notebook, I had to implement a timeout exception in one of the functions, because some multiple choice answers were stalling the function. So, I ignored some of them based on the time taken to add dummies for them.

4. Model Data

For questions 1 and 2, there was no need for machine learning, but I had to build a new dataframe with only language or platform information and then model it to show me the ranking of each language or platform in each year.

For question 3, I used the LinearRegression model of sklearn, after cleaning the data for each of the years.

5. Results

Results are the findings from the wrangling and modeling. They are the answers I found to each of the questions. And for each of the answers, some kind of visualization (graphs and/or tables) of the results was built.

6. Deploy

The deployment process was to create this github repository and then the medium post, describing the results, which you can find in the results section.

## File Descriptions <a name="files"></a>

There are 3 notebooks available here to showcase work related to the above questions.  Each of the notebooks is exploratory in searching through the data pertaining to the questions showcased by the notebook title.  Markdown cells were used to assist in walking through the thought process for individual steps.

1. LanguageRankings.ipynb: Notebook that solve question 'a' and shows a final graph with the ranking evolution of each language between 2017 and 2019.

2. PlatformDesireRankings.ipynb: Notebook that solve question 'b' and shows a final graph with the ranking evolution of each platform between 2017 and 2019.

3. Coefficients.ipynb: Notebook that solve question 'c' and shows three graphs for the top 20 coefficients in the models for each of the years.

I also included the 3 datasets used (survey_results_public_yyyy.csv), but they are zipped as they were larger than GitHub's limit if not zipped.

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@madoreiraluizrv30/what-were-the-programming-trends-of-the-last-years-8c60d9225772), but here is a summary:

a. The three most used languages continued to be Java, Javascript and C, but C came ahead of the other two since 2018, and Objective C dropped many positions since 2017 (Swift becoming the go-to language on iOS development could be the reason, even though Swift ranking also decreased during the same time).

b. Linux, Windows, AWS and Android were always at the top of the rankings throughout the years (the only "intruder" was Docker in 2019), but Linux came ahead of the other ones since 2018, while Android dropped from first in 2017 to fourth in 2019. Windows is steadily going up on the ranking, so maybe on the next survey, it will be the number one.

c. Where an individual lives continued to be of the greatest indicators of salary throughout the years. But some different variables appeared as top indicators in different years: in the earlier years (2017 and 2018) years of experience were important, and in the later years (2018 and 2019) different techs used were relevant.

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

I have used a snippet of code found [here](https://stackoverflow.com/questions/366682/how-to-limit-execution-time-of-a-function-call-in-python) for the timeout exception function.

Must give credit to Stack Overflow for the data.  You can find more information at the link available [here](https://insights.stackoverflow.com/survey).  Otherwise, feel free to use the code here as you would like! And you have any feedback, please share



