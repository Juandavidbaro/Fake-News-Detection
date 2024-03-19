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

# Next steps
## Data preparation
In order to be able to use the texts in a model it will be necessary to process them so that they are converted into numerical values that represent only the really necessary parts of the information. The following are planned to be included:
### Stemming
Words are transformed at their root to facilitate the following processes that abstractly reduce words to quantifiable values.
### Lemmatization
This is a similar process to the previous one and serves the same purpose. However, instead of employing rules to arrive at the root of a word, dictionary-like mechanisms are used to convert words into other words that drive their meaning within the model. For example: Changing can become chang (stemming) or change (lemmatization).
The above processes will be considered as mutually exclusive, it is not yet defined which of them will be applied to the dataset as the choice is subject to the effectiveness of the model when one or the other is applied.
### Stopwords
Stopwords are words that have no meaning when they are not accompanied by other words. That is, words that can be ignored in the analysis because they do not provide any kind of value or meaning within the model.
### Tokenization
This is the process of converting text into smaller units that can be analyzed by the model. This process varies according to the implementation and is quite abstract, since, given a dictionary of words the resulting set of tokens could correspond to subwords, characters or character strings that while they have no meaning for us as readers, they do have meaning for the model; the purpose is to take the text from our language to one that the machine is able to process.
## Training and evaluation
Once the data is prepared, the process of training, evaluating and tuning the model to maximize the established metrics will begin.
## Deployment
The last planned step is to deploy the model so that it can be used by end users. This could involve connecting it to a web application that serves as an interface and facilitates user tasks such as submitting the title and content of the news item to be reviewed.
Because of the above, it is possible that some web stack or other technology other than python and jupyter notebook may also need to be included for the sole purpose of making the model accessible.

## Additional data
To obtain additional data and improve the quality and diversity of your dataset for your fake news detection project, the following techniques can be used:

- **Web Data Extraction:** Develop scripts to extract news data from multiple online sources. This allows you to gather a wide variety of articles from different news websites.

- **Crowdsourcing:** Utilize crowdsourcing platforms where individuals can contribute by labeling data. You can ask users to classify news articles as fake or real, providing you with a large-scale labeled dataset.

- **Collaboration:** Establish collaborations with other organizations or researchers who may have access to relevant datasets. This allows you to expand your resources and obtain additional high-quality data.

- **Data Augmentation:** Implement data augmentation techniques to generate new samples from your existing data. This may include techniques such as back translation, paraphrasing, and introducing small variations in the text.

- **Social Media APIs:** Use APIs provided by social media platforms to collect news data shared on these platforms. Social media is a rich source of news and opinions that can enrich your dataset.

## Ethical Considerations:

When implementing artificial intelligence solutions for fake news detection, it is essential to consider a range of ethical aspects. This includes ensuring transparency and explainability of the models used, mitigating biases and ensuring fairness in the outcomes, safeguarding the privacy and personal data of users, taking responsibility for the social and cultural impact of these technologies, being transparent about the origin of the data used, and committing to ongoing evaluation and improvement of the systems. By addressing these ethical considerations, responsible and ethical use of artificial intelligence in combating fake news can be promoted, safeguarding the rights and trust of users.

