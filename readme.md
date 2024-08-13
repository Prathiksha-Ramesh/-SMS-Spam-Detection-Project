# SMS Spam Detection Project

This repository contains the source code and resources for the **SMS Spam Detection** project. The project uses machine learning techniques to classify SMS messages as spam or ham (not spam). The dataset used for this project is the "SMSSpamCollection," which is a collection of SMS messages labeled as spam or ham.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [Contact](#contact)

## Project Overview

The **SMS Spam Detection** project involves using natural language processing (NLP) techniques and machine learning algorithms to build a model that can classify SMS messages as spam or ham. The key steps in this project include:

- Data loading and preprocessing
- Exploratory Data Analysis (EDA)
- Feature extraction
- Model training and evaluation
- Model deployment (if applicable)

## Dataset

The dataset used in this project is the **SMSSpamCollection**, which contains SMS messages labeled as spam or ham. The dataset is preprocessed to remove stopwords, punctuation, and to convert text to lowercase.

## Project Structure

- **notebook.ipynb**: The Jupyter notebook containing the complete code for data preprocessing, model training, evaluation, and visualization.
- **SMSSpamCollection**: The dataset file containing labeled SMS messages.
- **LICENSE**: The Apache License 2.0 file that governs the use and distribution of this project's code.
- **requirements.txt**: A file listing all the Python libraries and dependencies required to run the project, including Numpy, Seaborn, Matplotlib, Scikit-learn, and Pandas.
- **.gitignore**: A file specifying which files or directories should be ignored by Git.

## Installation

To run the project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone repository link
``` 

2. Navigate to the project directory:

``` bash 
cd your-repository-name
```

3.Create a virtual environment (optional but recommended):

``` bash 
python3 -m venv venv
source venv/bin/activate   # On Windows use `venv\Scripts\activate`
```

4.Install the required dependencies:
``` bash 
pip install -r requirements.txt
```

5.Run the Jupyter notebook:
``` bash 
jupyter notebook notebook.ipynb
``` 
## Usage
To use this project, you can run the Jupyter notebook to preprocess the data, train the model, and evaluate its performance. The notebook provides step-by-step instructions and code explanations.

## License
This project is licensed under the Apache License 2.0. See the `LICENSE` file for more details.

## Contact
For any inquiries or contributions, feel free to reach out or submit an issue or pull request on GitHub.

