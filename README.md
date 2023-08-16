# Topic Modeling and Classification of Customer Reviews

This project focuses on utilizing Latent Dirichlet Allocation (LDA) for topic modeling and Support Vector Machine (SVM) for classification of customer reviews. In addition, a heuristic-based post-processing method has been applied to enhance the accuracy of the classification results.

## Table of Contents

- [Introduction](#introduction)
- [Methods](#methods)
- [Project Structure](#project-structure)
- [Results](#results)
- [Conclusion](#conclusion)
- [Acknowledgements](#acknowledgements)

## Introduction

In this project, we aimed to analyze and classify customer reviews to identify the main topics of discussion. We leveraged Latent Dirichlet Allocation (LDA), a topic modeling technique, to extract latent topics from the text data. We further improved classification accuracy by combining LDA with Support Vector Machine (SVM), a powerful machine learning algorithm.

The project also incorporates a heuristic-based post-processing method. This approach involves refining the predicted labels using specific keywords or phrases that are indicative of certain topics. This heuristic method aims to address instances where the initial classification might not capture all relevant aspects discussed by the customers.

## Methods

1. **Data Preprocessing**: The raw customer review data is preprocessed, including tokenization, removal of stopwords, and other text cleaning tasks.
2. **Latent Dirichlet Allocation (LDA)**: LDA is employed to extract latent topics from the reviews.
3. **Support Vector Machine (SVM)**: The LDA topic probabilities are used as features to train an SVM classifier.
4. **Heuristic Post-Processing**: After SVM classification, heuristic rules are applied to adjust the labels based on predefined keywords associated with specific topics.

## Project Structure

The project structure is organized as follows:


- `Customer Feedback Analysis`: Contains raw review data.
- `adjusted.xlsx and output.xlsx`: Contains processed review data with and without heuristics respectively.
- `combo.ipynb`: Jupyter notebook containing the main workflow of LDA and SVM integration.
- `lda_model_saved and svm_model.pkl`: Holds saved LDA and SVM model files.
- `check_adj.xlsx and check_df.xlsx`: Contains data showing processed review labels against original labels used to measure performance.
- `requirements.txt`: Lists the required libraries and packages for the project.


## Results

The project achieved significant success in accurately classifying customer reviews into relevant topics. The LDA model effectively extracted latent topics, which were used as features for SVM classification. The heuristic-based post-processing improved the overall classification accuracy, especially in cases where certain keywords were indicative of specific topics.

## Conclusion

This project showcases the power of combining natural language processing techniques with machine learning algorithms for effective topic modeling and classification of customer reviews. By integrating LDA and SVM, along with a heuristic-based approach, the project demonstrates an innovative method to extract insights from customer feedback.

## Acknowledgements

I would like to express my gratitude to the open-source community for providing essential libraries and tools that enabled the successful completion of this project.
