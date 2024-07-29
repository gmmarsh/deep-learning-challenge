# Deep Learning for Binary Classification
The purpose of this analysis is to develop a binary classification model that will assist Alphabet Soup with selecting applicants for funding that will have the best chance of success in their ventures. The model will predict if the venture will be successful or not sucessful.

## Table of Contents
- [Introduction](#introduction)
- [Data](#data)
- [Methodology](#methodology)
- [Results](#results)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
In the context of this project, a deep learning model can help Alphabet Soup accurately predict the success of ventures based on historical data, thereby making informed fuding decisions.

Deep learning neural networks are valuable because of their ability to learn complex patterns, reduce the need for feature engineering and to scale as more data becomes available.

## Data
The dataset used for this project consists of a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as application type, affiliation, classification, use-case, organization type, status(active or inactive), income amount, the ask amount and "is_succesful" (was the money used effectively).

The target variable for the model is the "IS_SCCESSFUL" lable.

The feature varialbes for the model are APPLICATION_TYPE—Alphabet Soup application type, AFFILIATION—Affiliated sector of industry,CLASSIFICATION—Government organization classification, USE_CASE—Use case for funding,ORGANIZATION—Organization type, STATUS—Active status INCOME_AMT—Income classification,SPECIAL_CONSIDERATIONS—Special considerations for application, ASK_AMT—Funding amount requested

EIN and NAME—Identification columns were removed from the input data because they are neither target nor features.

## Methodology
Step 1 consisted of preprocessing  the CSV data using Pandas and scikit-learn's StandardScaler.

Step 2 consisted of compiling, training and evaluating two neural network models: a base model and an optimized model.

Step 3 consisted of optimizing the neural network model.

Step 4 consisted of a written report on the performance of the deep learning model used.

## Results
The second optimized model produced a test accuracy of 0.7289 which is slightly higher than the test accuracy of the starter code base model of 0.7287.To improve the base model performance, the number of neurons changed from 80 to 128. In the second layer, the number of neurons increased from 30 to 64. An additional hidden layer was also added with 32 neurons and a relu activation function. A dropout of .5 was also added to each layer to help reduce overfitting.

## Usage
To use this project, follow these steps:
1. Clone the repository: `git clone https://github.com/gmmarsh/deep-learning-challenge.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Run the main script: `Starter_Code.ipynb` and `Optimization.ipynb`

## Contributing
Contributions to this project are welcome. If you find any issues or have suggestions for improvement, please open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.