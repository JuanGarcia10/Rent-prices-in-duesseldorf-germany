# Introduction and motivation

The following is an analysis of the rent prices in Germany, specially for the capital of Nordrhein-Westfalen (Düsseldorf)

I am interested in the behavior of rent prices for Düsseldorf and aim to answer the following questions:
1. How expensive is to live in Düsseldorf compare to any other city in Nordrhein-Westfalen (NRW)?
2. How is the distribution of rent prices in the city? if we look for a specific borough/neighborhood and a given size?
3. How do the characteristics of a flat explain the variability in prize?
4. Can the rent prices in Düsseldorf be accurately predicted using a linear model?

***A summary of my findings*** can be found in my blog-post in Medium - [please follow this link for free reading](https://medium.com/@juangarcia10/predicting-rent-prices-in-germany-how-expensive-is-really-d%C3%BCsseldorf-63484e4bf658?sk=e772554443a2cbf36fc279ab7d39038d)

# About the Notebooks

I follow the CRISP-DM process and divided my work into three notebooks for a better structured:
* "Data_cleaning_rent_flats_germany" reflects the first steps of CRISP-DM, i.e. Business understanding, data understanding, and data preparation
* "Data_exploration_flats_germany" reflects the modeling part of CRISP-DM, i.e. understanding the variables better and setting the model
* "Graphics_for_article" is the final touch to the modeling and evaluation part of CRISP-DM, i.e. polishing the results, fitting the final model and evaluating it. No deployment part is included as the project is not meant to be deployed to any system

# About the Dataset and Acknowledgments

I am working with the dataset "immo_data.csv" from kaggle. This dataset contains information about the apartment (flats) rental offers in Germany. It was created by "CorrieBar" from the popular German website Immoscout24. It contains all published offers from 3 different days during 2018 and 2019. ***Please refer to Kaggle to get the data, as I did not include it in the repository***. [Just follow the link](https://www.kaggle.com/corrieaar/apartment-rental-offers-in-germany)

# Methodology

I use Python 3.* for the analysis.
Libraries used:
```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import r2_score, mean_squared_error
```
