# Research Questions

- How can fake news be differentiated from real news using textual data?
- What linguistic or content characteristics are indicative of fake news?
- Are there temporal or geographical patterns in the propagation of fake news?
- How do the characteristics of fake news vary between topics?

# Problem Type

This project is a binary classification problem in supervised learning, where the goal is to predict if a news article is fake or true.

# Methodology

The project will be based on the CRISP-DM methodology:
1. Business Understanding: Define clear objectives, understand the project's impact.
2. Data Understanding: Gather datasets of different news articles, explore quality, diversity, and truthfulness.
3. Data Preparation: Select relevant news articles, perform cleaning, and augment data if necessary.
4. Modeling: Select and apply deep learning models such as convolutional neural networks (CNNs), adjust parameters, and train the model.
5. Evaluation: Review the model's performance using specific metrics, compare it with the objectives.
6. Deployment: Implement the model in a production environment, plan for its maintenance and updates.

# Metrics

The most suitable evaluation metrics for this type of project include:
- Accuracy: Proportion of correct predictions over the total.
- Recall: Model's ability to find all relevant instances.
- F1-Score: Harmonic mean of precision and recall, useful when classes are imbalanced.
- AUC-ROC: Area under the ROC curve, measures the model's ability to distinguish between classes.

# Databases to Use

The data to be used are Fake News Detection Datasets:
[Link to Kaggle](https://www.kaggle.com/datasets/emineyetm/fake-news-detection-datasets)
