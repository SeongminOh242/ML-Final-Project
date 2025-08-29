🎨 PPG Paint Colors: Machine Learning Final Project
Overview

This project applies machine learning techniques to study paint color data provided by PPG Industries, the world’s largest coatings company. Using PPG’s real dataset of paint colors, we explore how color model inputs (RGB and HSL) influence:

A continuous paint property (response, transformed using logit).

A binary popularity outcome (outcome: 1 = popular, 0 = less popular).

The project combines exploration, regression, classification, and interpretation, providing a full end-to-end data science workflow.

⚠️ Important Notice:

The dataset is proprietary and cannot be shared on GitHub, blogs, or public repositories.

You may share your models, preprocessing code, and methodology, but not the raw data, feature importance rankings, or proprietary conclusions.

Project Tasks
🔎 Part I: Data Exploration

Visualize variable distributions (histograms, density plots).

Examine differences in distributions across categories and binary outcomes.

Study correlations between inputs (RGB, HSL) and outputs (response, outcome).

📈 Part II: Regression

Goal: Predict logit-transformed response.

Linear Models (lm)

Fit 10 variations (intercept-only, categorical-only, continuous-only, interactions, basis functions, etc.).

Compare performance and visualize top 3 models’ coefficients.

Bayesian Linear Models (stan_lm, stan_glm)

Fit 2 models (best from above + one alternative).

Analyze posterior uncertainty on coefficients and error variance.

Predictions

Visualize predictive trends with confidence and prediction intervals.

Advanced Models with Resampling

Elastic Net, Neural Networks, Random Forest, Gradient Boosted Trees, and 2+ custom methods.

Compare models using chosen resampling scheme and metrics (RMSE, R², etc.).

🧮 Part III: Classification

Goal: Predict paint popularity (outcome).

Generalized Linear Models (glm)

Fit 10 variations (similar structure as regression).

Compare top 3 and visualize coefficients.

Bayesian GLMs

Fit 2 models (best + one alternative).

Analyze posterior uncertainty and predictive performance.

Predictions

Visualize event probability trends with confidence intervals.

Advanced Models with Resampling

Elastic Net, Neural Networks, Random Forest, Gradient Boosted Trees, and 2+ custom methods.

Compare models on Accuracy vs ROC AUC.

🔍 Part IV: Interpretation

Identify best regression and classification models.

Determine most important inputs (RGB vs HSL features).

Explore hardest and easiest to predict paints.

Visualize predictive surfaces for combinations of Lightness & Saturation.

Bonus Opportunities

PPG Presentation: Create a presentation of results (+10 points).

Synthetic Data with Bayesian Models: Demonstrate recovery of known parameters (+15 points).

Low-Frequency Categories: Handle rare categorical inputs using recipes (+10 points).

Imbalanced Data: Apply subsampling to rare-event classification (+15 points).

Tools & Libraries

Language: R

Packages:

caret or tidymodels for modeling, resampling, and tuning

boot for logit transformation

rstanarm for Bayesian modeling

ggplot2 for visualization

Submission: .Rmd source files + rendered .html reports

Deliverables

RMarkdown (.Rmd) source files (split by project parts)

Rendered HTML documents (uploaded separately)

Predictions on test set (to be released in April)

📅 Deadline: April 17, 2024

References

PPG Industries

PPG Paint Tools

Tidymodels

Caret Models List

Interpretable ML Guide
