# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

> **Your Answer:**
In this scenario we have a regression problem because we want to predict a numerical value, which factors affect species richness (response). We are interested in inference because we care about interpreting relationships. 
The observation of the dataset is n = 200, one observations per marine reserve with p = 4 predictors (reserve size, year since establishment, enforcement budget, proximity to human settlements). 

---

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and eight other variables.

> **Your Answer:**
The response is successful vs unsuccessful wildlife movement making it a catagorical outcome, classification problem. The agency wants accuret predictions for new cases to propose if corridors will succeed. 
n = 30 observations and p = 11 (corridor width, length, surrounding land suse type, 8 additional variables)
---

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric

> **Your Answer:**
This scenario we have a regression problem. The response is weekly average ozone concentration, a coninuous numeric variable. we are most interested in predictions because the task is to predict ozone levels. n = 52 because weekly data for one year. p = 4 sea surface temperature, wind speed, solar radiation, and atmospheric variable.
---

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

> **Your Answer:**
Advatages of very flexible approach for regression can capture nonlinear relationships and complex interactions and can achieve higher predictive accuracy when the true relationship is complicated. Lower bias. 

Disadvantages are higher variance lead to overfitting, harder to interpret, and requires more data to perform well 

---

### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

> **Your Answer:**
A parametric approach assumes a specific functional form for the relationship between predictors and the response. This means the model can be summarized using a fixed number of parameters. In contrast, a non-parametric approach makes fewer assumptions about the functional form and instead allows the data to determine the shape of the relationship, often resulting in more flexible models.

Advantages of parametric approaches
- They are simpler and easier to interpret, ideal for inferences.
- Good for small datasets, they need to estimate less parameters.
- Computationally efficient.

Disadvanatage of parametric approaches
- They impose strong assumptions, for example linearity, which may not reflect the true relationship.
- They have high bias if the model is misspecified, leading to underfitting.
- They are less able to caputre complex or nonlinear patterns in the data compared to non-parametric methods

In general parametric methods trade flexiblity for simplicity and intepretability, while non-parametric methods offer flexibility at the cost of requiring more data and being harder to interpret. 