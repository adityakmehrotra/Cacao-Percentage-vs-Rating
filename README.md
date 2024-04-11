# Cocoa-Percentage-vs-Rating
Using Machine Learning and Analysis to determine the relationship between the cocoa percentage of a type of chocolate and its objective rating.

## Introduction

A universally popular treat, chocolate is available in a variety of forms ranging from beverages, pastries, ice creams, and of course, the standard chocolate bar. In the United States alone, an estimated average of 2.8 billion pounds of chocolate are consumed each year! Milk chocolate is the American fan favorite, with a usual cacao percentage range of 10-55%, followed by Dark Chocolate, with a cacao percentage of at least 55% and above. Between these two popular types of chocolate, cacao percentage helps distinguish the sweeter and lighter tastes of the Milk Chocolate from the richer, more bittersweet taste of Dark Chocolate. Simply put, cacao percentage is the ratio between actual cacao product from cacao butter, liquor, and powder and filler ingredients like vanilla, milk, and other added flavors. Generally, a higher cacao percentage denotes a more intense taste and higher price point, implying that it is of higher quality. Given this information, is it fair to say that higher quality chocolate yields higher ratings? Our study explored whether cacao percentage has a large influence on chocolate ratings in addition to using cacao percentage as a predictor for such chocolate ratings.

### Thesis

While higher cacao percentage is predicted to lead to a lower chocolate rating, there does not appear to be a strong relationship between those two variables.

## Background

### Dataset Information

This dataset includes 2,600 ratings of plain (non-flavored) chocolate bars produced by chocolate manufacturers around the world. The ratings are conducted by the Manhattan Chocolate society, who conduct research on chocolate production in order to produce innovative, high quality chocolate.

In the original Chocolate dataset, 7 variables are mentioned: REF (manufacturing number), Company (Manufacturer) Name, Company Location, Review Date, Country of Bean Origin, Specific Bean Origin or Bar Name, Cacao Percentage, Ingredients, Most Memorable Characteristics, and Rating. For the purposes of our study, we will consider 2 of the 7 variables: **Cacao Percentage, and Rating.**

#### Data Collection

##### Rating Column

Each row in the dataset represents one rating for one brand of chocolate bar. Ratings were conducted by members of the Manhattan Chocolate Society, comprising of chocolate authors, makes, and experts--people involved in the chocolate industry for an extensive amount of years. Ratings were conducted on a five point scale:

**1.0 - 1.9: Unpleasant**

**2.0 - 2.9: Disappointing** 

**3.0 - 3.49: Recommended**

**3.5 - 3.9: Highly Recommended**

**4.0 - 5.0 : Outstanding**

To determine the rating, the below factors were considered:

**Flavor:** How intense the cacao tastes (mild-moderate-strong), the roast of the chocolate,       dominant ingredients (cacao, sugar, butter) or if the ingredients are balanced, the             profile (floral, fruity, herby, smokey notes), and bitterness (mild-moderate-strong)

**Texture:** a higher quality chocolate will have a creamier, more even consistency, whereas       a lower quality chocolate will be more gritty, waxy, and dry

**Aftermelt:** the lasting experience/taste of the chocolate after it has melted in your mouth. A higher quality chocolate will have a longer lasting pleasant flavor, whereas lower quality chocolate not have as long lasting of an aftertaste and possibly leave an astringent, or acidic by-product.

##### Cacao Percentage

Cacao percentage present in each chocolate bar was given by the manufacturer of that chocolate bar. The Manhattan Chocolate Society reviews chocolate from companies that are transparent about their production process.

### Possible Counfounding Factors
Since all the ratings of the chocolate bars were performed by members of the Manhattan Chocolate Society, their ratings are in part influenced by each member's subjective taste standards. Thus,
the results of this study are only application to members of the society and not representative of the general population.

### Our Objective
In the rest of the report, we will analyze the relationship between cacao percentage and chocolate ratings using the provided dataset. Our primary question is whether the cacao percentage significantly influences the chocolate ratings. We will explore graphical representations, statistical analyses, and draw inferences based on the data.

## Analysis

To measure the relationship between cacao percentage and chocolate ratings, a simple linear model was constructed. 

<img width="914" alt="Screenshot 2024-04-11 at 3 39 39 PM (2)" src="https://github.com/adityakmehrotra/Cocoa-Percentage-vs-Rating/assets/24847438/05a05a59-8570-455c-b175-c6947c5d82b7">


**Null hypothesis**: The percentage of cacao in a chocolate bar does not affect its ratings, the slope of the linear regression model will be 0.

$H_0: \beta_1 = 0$ 

**Alternative hypothesis** The percentage of cacao in a chocolate bar does affect its ratings, the slope of the linear regression model will not be 0.

$H_a: \beta_1 \neq 0$
