# Fake-News-Detection

**Members:**
- Juan David Bahamon
- Samuel Hernandez
- David Peñaranda

## Context of the Problem:

In today's digital era, the rise of fake news has become a significant problem. These deceptive stories can negatively impact society, influencing what people think, decide, and do. It's crucial to detect and halt the spread of these fake news stories to ensure that the information we receive is reliable and truthful, thereby promoting an environment of honesty and trustworthiness in information dissemination.

## Project description:

The project focuses on developing a fake news detection system using machine learning techniques, specifically in the realm of binary classification. The aim is to build a model capable of distinguishing between real and fake news using textual data as input. This involves identifying linguistic and content characteristics that can differentiate between genuine and falsified news articles.

### Next steps
### Data preparation
In order to be able to use the texts in a model it will be necessary to process them so that they are converted into numerical values that represent only the really necessary parts of the information. The following are planned to be included:
#### Stemming
Words are transformed at their root to facilitate the following processes that abstractly reduce words to quantifiable values.
#### Lemmatization
This is a similar process to the previous one and serves the same purpose. However, instead of employing rules to arrive at the root of a word, dictionary-like mechanisms are used to convert words into other words that drive their meaning within the model. For example: Changing can become chang (stemming) or change (lemmatization).
The above processes will be considered as mutually exclusive, it is not yet defined which of them will be applied to the dataset as the choice is subject to the effectiveness of the model when one or the other is applied.
#### Stopwords
Stopwords are words that have no meaning when they are not accompanied by other words. That is, words that can be ignored in the analysis because they do not provide any kind of value or meaning within the model.
#### Tokenization
This is the process of converting text into smaller units that can be analyzed by the model. This process varies according to the implementation and is quite abstract, since, given a dictionary of words the resulting set of tokens could correspond to subwords, characters or character strings that while they have no meaning for us as readers, they do have meaning for the model; the purpose is to take the text from our language to one that the machine is able to process.
### Training and evaluation
Once the data is prepared, the process of training, evaluating and tuning the model to maximize the established metrics will begin.
### Deployment
The last planned step is to deploy the model so that it can be used by end users. This could involve connecting it to a web application that serves as an interface and facilitates user tasks such as submitting the title and content of the news item to be reviewed.
Because of the above, it is possible that some web stack or other technology other than python and jupyter notebook may also need to be included for the sole purpose of making the model accessible.
 
 
