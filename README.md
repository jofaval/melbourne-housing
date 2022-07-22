# Melbourne Housing Exploration and Estimations #

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jofaval/pima-indian-diabetes/blob/master/notebook.ipynb)&nbsp;[![Open in Kaggle](https://www.kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/jofaval/melbourne-housing-exploration-and-estimations-0-86)

## Table of contents

1. [📁 Data](#-data)
1. [📓 Description](#-description)
1. [✔️ Objective](#-objective)
1. [🧱 Tech stack](#-tech-stack)
1. [💹 Algorithms](#-algorithms)
1. [📊 Visualization](#-visualization)
1. [🤓 Conclusions](#-conclusions)
1. [©️ Credits](#-credits)

## 📁 Data
[↑ Back to the table](#table-of-contents)

The data is available at the official link:\
[https://www.kaggle.com/datasets/dansbecker/melbourne-housing-snapshot](https://www.kaggle.com/datasets/dansbecker/melbourne-housing-snapshot)

The original dataset is available at:\
[https://www.kaggle.com/datasets/anthonypino/melbourne-housing-market](https://www.kaggle.com/datasets/anthonypino/melbourne-housing-market)

## 📓 Description
[↑ Back to the table](#table-of-contents)

It was scraped from publicly available results posted every week from Domain.com.au. He cleaned it well, and now it's up to you to make data analysis magic. The dataset includes Address, Type of Real estate, Suburb, Method of Selling, Rooms, Price, Real Estate Agent, Date of Sale and distance from C.B.D.

## ✔️ Objectives
[↑ Back to the table](#table-of-contents)

Melbourne real estate is BOOMING. Can you find the insight or predict the next big trend to become a real estate mogul… or even harder, to snap up a reasonably priced 2-bedroom unit?

What I ended up doing was, some data analysis to gain some insights and hypothesize a little bit. And create models using machine learning techniques to predict/estimate the real state price (having an almost perfect score in housing would not be the best option, since you'll be working with estimates, not exact numbers, which is something to take into account, at least from my own perspective).

## 🧱 Tech stack
[↑ Back to the table](#table-of-contents)

Python, that's it! R is a programming language that, as for the moment being, I have no experience with, even though it's powerful and broadly used, but I'd dare to say that no more than Python.

And one of the strongest points, if not the most, about Python, are it's libraries, so... the libraries I've used are:

- Pandas, data manipulation with an ease of use and exploration data analysis.
- Numpy, a really strong linear algebra library, used in the project for it's statistics utilities, SciPy may be an alternative, but I have no experience at all with it.
- Matplotlib and Seaborn, both fantastic libraries for data visualization, and they complement each other.
- Scikit-Learn, the library used for Machine Learning and statistics models: Linear Regression, SVR, Lasso, Ridge, etc.
- Tensorflow and Keras, the industry standard for Deep Learning, the way to go, not really, it's just that for now I don't have that many experience with PyTorch

## 💹 Algorithms
[↑ Back to the table](#table-of-contents)

I've used quite a few algorithms, I had the idea in mind of just Linear Regression and XGBoost, but then I decided to try my luck with a few others (it was just to test their performance a little bit)

- **Linear Regression**: the simplest, but quite effective technique.
- **XGBoost**: a complex unsupervised technique quite popular and effective. It performed the best.
- **Random Forest**: a forest of decision tree where the fittest survives, literally.
- **Decision Tree**: a single decision tree that branches different possibilities.
- **Dense Neural Network**: a fixed set of units and activation functions with hidden layers between inpuut and output.
- **LightGBM**: a distributed gradient-boosted technique, it was the second best technique for this dataset.
- **Bayesian Ridge/Lasso**: I group them together since they had the exact same performance, what differs from classic linear regression it's the regulaization, kind of.
- **Single Shot**: similar to a dense neural network, but without any hidden layers, this time it performed a little bit better than the DNN, which is usually not the case.

## 📊 Visualization
[↑ Back to the table](#table-of-contents)

What I struggled with the most, to the point that I even forgot how to do it, was to represent what was trying to be predicted/estimated, which is as simple as a scatterplot of the regression target value.

Actually analyzing the distribution of the price helped me realize that the most expensive houses, those outliers value, were breaking the model, they were most likely adding a ton of error that shouldn't even be there. So there's a comparison between what was the actual house market and what my best model (XGBoostRegressor) predicted, which is, by far, much smoother.

## 🤓 Conclusions
[↑ Back to the table](#table-of-contents)

Housing datasets are hard to work with and to actually make a good analysis on, well, so is every other dataset, domain knowledge is sooo important. Working with missing values is always something risky, I did my best to fill the gaps as best as I could, but that's something I feel that made this project, and it's resolutions, incosistent, as in, it may make statistical sense, but there's no better value than the real one.

And this dataset was just astonishing, I mean, it's a good set of values put together, and it was nice to have it free and highly available. Even though there's missing values, there're quire some features that are nicely explained at the dataset page.

## ©️ Credits
[↑ Back to the table](#table-of-contents)

Created originally by [Tony Pino](https://www.kaggle.com/datasets/anthonypino).

Uploaded at Kaggle, a company owned by Google, by [https://www.kaggle.com/dansbecker](https://www.kaggle.com/dansbecker).