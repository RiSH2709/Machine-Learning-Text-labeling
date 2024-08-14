 📚 NotTheRealWikipedia Content Analysis Project

 Overview
This project was developed for a non-profit organization, NotTheRealWikipedia, to explore how machine learning can be leveraged to enhance the content on their platform. The project focuses on two key tasks:
1. Topic Classification: Automatically identify the topic of a paragraph-sized text.
2. Clarity Detection: Assess whether a given paragraph is written clearly enough.
 Tools and Techniques Used
1.	Python Environment: All data processing, model development, and evaluation were performed using Python.
2.	Excel: Used for initial data exploration and basic cleaning tasks.
3.	Web Scraping: Gathered additional data from the internet to enhance the dataset.
4.	Machine Learning Models: 
-	Task 1: Naive Bayes for topic classification.
-	Task 2: Logistic Regression for clarity detection.

 Project Structure
- content_analysis.py: The main Python script containing the code for both tasks, including data preprocessing, model training, and evaluation.
- data/: Contains datasets used throughout the project.
  - `original_dataset.csv`: The original, uncleaned, and unlabelled dataset provided for the project.
  - `final_df.xlsx`: The cleaned and filtered dataset, including the 100 labeled data points used for clarity detection.
- notebooks/: Jupyter notebooks detailing additional analysis, feature engineering, model development, and evaluation.
 Task 1: Topic Classification
 Objective
Classify a paragraph into one of the following categories:
- Artificial Intelligence
- Movies about Artificial Intelligence
- Programming
- Philosophy
- Biographies
 Approach:
- Input Features: Utilized the paragraph text and an entity detection feature (`has_entity`).
- Modeling: Used Naive Bayes, with extensive hyperparameter tuning.
- Evaluation: Focused on ensuring low misclassification rates, especially avoiding unrelated class errors.
 Results:
- Achieved a model that outperformed a trivial baseline, with a balanced accuracy across the five categories.
- Used metrics such as F1-score and confusion matrix to assess the model's performance.

 Task 2: Clarity Detection
 Objective
Develop a prototype to predict whether a paragraph is "clear_enough" or "not_clear_enough."
 Approach
- Labeling: Manually labeled a subset of 100 data points for clarity, which are stored in the `final_df.csv` file.
- Modeling: Implemented Logistic Regression and explored techniques like pre-trained word embeddings and semi-supervised learning.
- Ethical Considerations: Addressed potential biases in automatic text rejection and suggested mitigation strategies.
 Results
- The model was able to predict clarity with accuracy surpassing the majority class baseline.
- Further suggestions were provided to improve the model, such as expanding the labeled dataset and applying transfer learning.
 Ethical Considerations
- Bias Mitigation: Discussed the risks of using automated systems to reject user-generated content and proposed alternative approaches.
- Responsible AI: Emphasized the importance of fairness and transparency in deploying machine learning models.
 Future Work
- Model Improvements: Incorporating more sophisticated NLP techniques and expanding the labeled dataset.
- Deployment Considerations: Exploring the integration of these models into the NotTheRealWikipedia platform while maintaining ethical standards.
 Contributing
Contributions are welcome! Feel free to fork the repository and submit a pull request with your improvements.

