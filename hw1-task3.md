# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

> **Your Answer:**

This is a regression problem and we are interested in inference. 
n = 200
p = 4 

---

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and eight other variables.

> **Your Answer:**

This is a classification problem and we are interested in prediction. 
n = 30
p = 11

---

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric

> **Your Answer:**

This is a regression problem and we are interested in prediction. 
n = 52
p = 4

---

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

> **Your Answer:**

Advantages: Can fit many different type of functional forms for f. 

Disadvantages: Can lead to overfitting data - follow noise in data too closely. Harder to interpret. 

A more flexible approach may be preferred when prediction is the goal - interpretability not a priority. 

A less flexible approach may be preferred when inference is the goal - would be easy to understand relationship between y and x1, x2, x3 etc. 
---

### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

> **Your Answer:**

**Parametric** statitsical learning approach: involve a two-step model based approach. 

1) Assumption about the functional form, shape of f is made. 
2) After model is selected, use training data to fit or train the model and estimate the parameters B0, B1, B2 etc. 
In summary, the parametric model-based approach reduces the problem of estimating f down to estimating a set of parameters. 

**Non-parametric** statistical learning approach: do not make explicit assumptions about the functionnal form of f - seek an estimate of f that gets as close to data points without being too 'rough' or 'wiggly'. Can more accurately fit a wider range of possible shapes for f. 

**Advanatges of paramatric approach**: More interperatable. 

**Disadvantages of paramtetric approach**: The model we choose will generally not match the true unknown form of f. Can only produce small range of shapes to estimate f. 