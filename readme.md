# SMS Spam Detection with Bag of Words and TF-IDF

This repository contains the source code and resources for an SMS Spam Detection project using Natural Language Processing (NLP) techniques such as Bag of Words and TF-IDF, along with machine learning models to classify SMS messages as spam or ham (not spam).

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
  - [Bag of Words Approach](#bag-of-words-approach)
  - [TF-IDF Approach](#tf-idf-approach)
- [Model Evaluation](#model-evaluation)
- [License](#license)
- [Contact](#contact)

## Project Overview

This project aims to classify SMS messages as spam or ham using two common text representation techniques: Bag of Words and TF-IDF (Term Frequency-Inverse Document Frequency). These representations are then fed into a Naive Bayes classifier to predict whether a message is spam or not.

## Dataset

The dataset used in this project is the **SMSSpamCollection**, which contains 5,574 SMS messages labeled as spam or ham. Each message has undergone text preprocessing to clean and normalize the data.

## Project Structure

- **notebook.ipynb**: The Jupyter notebook containing the complete code for data preprocessing, feature extraction (Bag of Words and TF-IDF), model training, evaluation, and visualization.
- **SMSSpamCollection**: The dataset file containing labeled SMS messages.
- **LICENSE**: The Apache License 2.0 file that governs the use and distribution of this project's code.
- **requirements.txt**: A file listing all the Python libraries and dependencies required to run the project, including NLTK, Gensim, Pandas, and Scikit-learn.
- **.gitignore**: A file specifying which files or directories should be ignored by Git.

## Installation

To run the project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/your-repository-name.git
```

2. Navigate to the project directory:
``` bash 
cd your-repository-name
``` 

3. Create a virtual environment (optional but recommended):

``` bash 
python3 -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
```

4. Install the required dependencies:

``` bash 
pip install -r requirements.txt
```

5. Run the Jupyter notebook:

``` bash 
jupyter notebook notebook.ipynb
``` 

## Usage

### Bag of Words Approach

- Text Preprocessing: The text data is cleaned by removing non-alphabetic characters, converting text to lowercase, tokenizing the text, removing stop words, and applying stemming using the Porter Stemmer.

### Bag of Words Model:

- A Bag of Words model is created using CountVectorizer with a maximum of 2,500 features and a n-gram range of (1,2).
- The text data is converted into a matrix of token counts.
- The processed data is split into training and testing sets.
- A Naive Bayes classifier (MultinomialNB) is trained on the training data and used to predict the test data.

## TF-IDF Approach
1. Text Preprocessing: Similar to the Bag of Words approach, but with lemmatization instead of stemming.

2. TF-IDF Model:

- A TF-IDF model is created using TfidfVectorizer with a maximum of 2,500 features and a n-gram range of (2,2).
- The text data is converted into a TF-IDF matrix.
- The processed data is split into training and testing sets.
- A Naive Bayes classifier (MultinomialNB) is trained on the TF-IDF data and used for predictions.

## Model Evaluation
The performance of the models is evaluated using the following metrics:

- Accuracy: The ratio of correctly predicted instances to the total instances.
- Classification Report: Provides precision, recall, and F1-score for both spam and ham classes.
- Confusion Matrix: To visualize the performance of the classification model.
The accuracy and other metrics are calculated to compare the effectiveness of the Bag of Words and TF-IDF approaches.

## License
This project is licensed under the Apache License 2.0. See the `LICENSE` file for more details.

## Contact
For any inquiries or contributions, feel free to reach out or submit an issue or pull request on GitHub.