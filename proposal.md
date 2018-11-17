# Project Proposal

## Project Description
This is a written description of your research project. Depending on the specifics of your project, you should outline the answers to these (and perhaps other) questions:

1. What is the overarching purpose of your research project, and why is it an important undertaking?

> The overarching purpose of our research project is to help students decide on what they want to major in college. By revealing potential relationships between majors and how much in salary people earn with their degrees, it will help kickstart the process of deciding on a major so students can have more time to learn rather than struggling to find a major of interest.

> It is an important undertaking because it is a topic that is closely related to us, college students who are actively seeking jobs and/or internships. If such information were accurately presented, it might affect students’ choices on majors because salary is, perhaps sadly, a very important factor when selecting a career.

2. How does your research fit into the broader problem domain? You should cite at least 3 papers that help contextualize your research.

> Student loan debt is quickly becoming a **national** problem (https://www.forbes.com/sites/tomlindsay/2018/05/24/new-report-the-u-s-student-loan-debt-crisis-is-even-worse-than-we-thought/#1a0e0de6e438)

> The authors from this research indicate that "few of them[college students] have good knowledge of what their earnings for their chosen field of study are likely to be." What we are doing in this project is to provide a better understanding of the future career paths and salary range of college majors. (http://www.hamiltonproject.org/papers/major_decisions_what_graduates_earn_over_their_lifetimes)

> This article shows a research about what motivates college students in choosing a major. According to this research, one of the top six factors in deciding upon a major is whether it "leads to a high paying job". Future income inevitably becomes an important factor when students decide a major. Through our project, we hope to demonstrate whether major decisions will affect students' lifetime salaries and whether there are significant salary differences between different majors. (http://www.nacadajournal.org/doi/10.12930/NACADA-13-018)

3. What specific hypothesis (hypotheses) are you going to test?

> Some specific hypotheses we are going to test are:
> - Does you choice of college and/or major(s) have a significant impact on your overall salary?
> - Are there any significant differences in job salary at different stages of your career because of your college and/or major(s)?

4. What are the datasets you'll be working with to answer this question? Please include relevant background describing the datasets you identify.

> The datasets we will be working with in order to answer our research questions come from here: “Where it Pays to Attend College" (https://www.kaggle.com/wsj/college-salaries). Though they are not so recent (last updated two years ago), they are from the Wall Street Journal, which is a credible source. It contains
> - degrees-that-pay-back.csv
> - salaries-by-college-type.csv
> - salaries-by-region.csv

> The main dataset we will be using is “degrees-that-pay-back.csv”. It contains various attributes like Undergraduate Major, Starting Median Salary, Mid-Career Median Salary, Percent change from Starting to Mid-Career Salary, etc. We will be able to utilize the data to understand the correlation between majors and salaries, and also the trend of salary growth.

5. What statistical and machine learning methods do you plan on using to test your hypothesis?

> We want to predict salary using majors, so we plan on using multiple linear regressions in order to test our hypotheses.
> - Use multiple indicators, college, major, etc., in order to predict salary for an individual
> - Linear regression will be useful because it allows us to measure the strength of impact of different indicators
> - Forward selection to determine the best possible variable combination for our model
> - Appropriate separation and use of training and test data
> - Cross-validation
> - Grid-search to optimize hyper parameters

6. Who is your target audience for the resource you will build? Depending on the domain of your data, there may be a variety of audiences interested in using the dataset. You should hone in on one of these audiences.

> Our main target audience will be students, who are concerned about how their decision on a college major will affect their future income. Parents and educators are some of our other audience as well because they play an important role in students’ decision making, but we will hone in on our student audience. We hope to provide resources for students to have a better understanding on their prefered majors using data science.

7. What should your audience learn from your resource? Consider specific questions they may want to answer.

> We hope our audience can learn the correlation, or the lack of, between majors and salaries. In addition, there are salary growths at different periods of a career, even if the career does not change. We will demonstrate how major decisions are generally affecting salaries. Some specific questions include:
> - Which majors get the highest salary in different periods (starting, Mid-Career, etc.)?
> - Which majors have the most salary growth?
> - How do salaries from different majors change over time?
> - What is the salary ceiling for different majors?


## Technical Description
This section of your proposal is an opportunity to think through the specific analytical steps you'll need to complete throughout the project.

1. What will be the format of your final web resource (Shiny app, HTML page or slideshow compiled with KnitR, etc.)?

> The format of our final web resource will be a HTML page.

2. Do you anticipate any specific data collection/data management challenges?

> The current datasets with three csv files might not be enough, so we anticipate challenges in finding more data for our research. Even if we could, we might encounter data management challenges because they are from different sources and might not be similar enough to be analyzed together.

3. What new technical skills will need to learn in order to complete your project?

> In order to complete our project, we will need to learn how to fetch external data using ways other than loading from a csv file. It is also a possibility for us to use more than one programming languages to deliver this report, so we will learn how to accommodate that as well.

4. How will you conduct your analysis? Please include a detailed description of your intended modeling approach.

> Like we mentioned above, we will use linear regression modeling for predicting salaries based on many variables and/or features such as regions, colleges, majors, etc. First things first, we will separate our entire dataset into training and testing data. We will then use forward selection to determine the best possible variable combination for our model. We also need to use cross-validation and then grid-search for tuning our hyper parameters.

5. What major challenges do you anticipate?

> A major challenge we anticipate is deciding which variables are most relevant to our goal. What if the existing variables are not relevant? We also anticipate difficulties in coming up with the “best” model because these data are time sensitive.