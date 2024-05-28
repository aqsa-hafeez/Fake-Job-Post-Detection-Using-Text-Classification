# Fake-Job-Post-Detection-Using-Text-Classification

# Abstract

This report explores the application of machine learning to detect fraudulent job postings. The project addresses the growing issue of deceptive job advertisements that waste job seekers' time and resources. We detail our methodology for training a text classification model on a balanced dataset of job postings labeled as fraudulent or legitimate. We evaluate the model's performance using various metrics and discuss its potential applications and limitations. Finally, we highlight areas for future work and key takeaways from the project.

# 1. Introduction

The online job market is crucial for connecting employers with potential employees. However, it has also become a breeding ground for fraudulent job postings, which aim to mislead job seekers with false promises. These deceptive advertisements can lead to significant losses of time and resources. Identifying and filtering out such postings is essential for protecting job seekers and maintaining the integrity of online job markets.
This report investigates the use of machine learning techniques for detecting fraudulent job postings. We present a text classification approach that analyzes the textual content of job postings to identify potential scams. By leveraging machine learning models, we aim to develop an automated system that can assist job seekers in navigating the online job market more safely and efficiently.
# 2. Problem Addressed

The primary problem addressed in this project is the detection of fraudulent job postings. Fraudulent job postings can mislead job seekers, leading to wasted effort and potential financial loss. By developing a machine learning model that can accurately distinguish between legitimate and fraudulent job postings, we aim to mitigate the impact of such scams.

# 3. Dataset Description

The dataset used in this project is a publicly available collection of job postings. It includes various features such as job title, company profile, job description, requirements, benefits, and a label indicating whether the posting is fraudulent (1) or legitimate (0). This dataset was preprocessed and balanced to ensure effective training and evaluation of the model.

# 4. Methodology Steps

The methodology for this project can be summarized in the following steps:

# 4.1 Data Preprocessing

We began by cleaning and preparing the raw dataset. This involved removing irrelevant characters (punctuation), converting text to lowercase, and tokenizing the text into individual words. Common stop words, which do not carry much meaning, were also removed.

# 4.2 Text Embeddings

We used pre-trained word vectors from the GloVe model to represent the meaning of each word in the text. These embeddings capture semantic relationships between words, allowing the model to understand contextual similarities.

# 4.3 Model Training

We trained a text classification model on the preprocessed data. We used a deep learning model with sequential layers, specifically a recurrent neural network (RNN) or convolutional neural network (CNN), to identify patterns in the text that distinguish fraudulent from legitimate job postings.

# 4.4 Model Evaluation

The trained model's performance was evaluated on a separate test set. We used metrics such as accuracy, precision, recall, and F1 score to assess the model's effectiveness in detecting fraudulent postings.

# 5. Application Area

This project has several potential applications:

# 5.1 Job Search Platforms

Online job boards can integrate the model into their platforms to filter out fraudulent postings before presenting them to job seekers. This can significantly improve the user experience and save job seekers time and effort.

# 5.2 Recruitment Agencies

Recruitment agencies can use the model to identify potentially fraudulent job postings before submitting applications on behalf of candidates, ensuring they focus on legitimate opportunities for their clients.

# 5.3 Individual Job Seekers

Individuals can leverage the model as a tool to assess the legitimacy of job postings before investing their time and effort. The model can be integrated into a browser extension or mobile app for real-time analysis.

# 6. Results and Findings

# 6.1 Data Visualization

We visualized the distribution of text lengths in job postings and the distribution of fraudulent vs. non-fraudulent postings. The data visualizations helped us understand the dataset better and informed our preprocessing steps.

# 6.2 Model Performance

The model's performance was evaluated using various metrics:

•	Training Accuracy: 1.0

•	Validation Accuracy: 0.995

•	Testing Accuracy: 0.993

The confusion matrices for training and testing sets are shown below: 
![image](https://github.com/aqsa-hafeez/Fake-Job-Post-Detection-Using-Text-Classification/assets/113436185/3de32958-c64f-47c6-845d-76a7fa9a6fc5)

![image](https://github.com/aqsa-hafeez/Fake-Job-Post-Detection-Using-Text-Classification/assets/113436185/fd44fdd3-90d7-4dc5-9e20-68d46204bb89)


These matrices indicate the model's ability to correctly classify fraudulent and legitimate postings.

# 6.3 Evaluation Metrics

•	Precision: Indicates the percentage of correctly identified fraudulent postings out of all identified as fraudulent.

•	Recall: Indicates the percentage of correctly identified fraudulent postings out of all actual fraudulent postings.

•	F1 Score: The harmonic mean of precision and recall.

# 7. Limitations

While the project demonstrates the potential of machine learning for detecting fraudulent job postings, some limitations exist:

# 7.1 Data Dependence

The model's performance relies heavily on the quality and representativeness of the training data. If the training data is biased towards certain types of fraudulent postings, the model may struggle to detect other types.

# 7.2 Emerging Scams

As scammers develop new tactics, the model may need to be retrained or adapted to detect new patterns in fraudulent postings. Regular updates with new examples of scams are crucial.

# 7.3 Explainability

The inner workings of complex models, such as deep learning models, can be difficult to interpret. This makes it challenging to understand why specific predictions are made, which can be a limitation in explaining the model's decisions.

# 8. Future Work

Several avenues exist for extending this project:

# 8.1 Exploring Different Models

Experimenting with alternative machine learning architectures, such as different RNN or CNN variations, may improve the model's performance. Ensembles of multiple models can also be explored.

# 8.2 Incorporating Additional Features

Expanding the model's feature set beyond textual content to include factors like company information (e.g., website existence) or salary offers compared to average salaries for the position might further enhance its accuracy.

# 9. Acknowledgements and Limitations

This project acknowledges the importance of data quality and the challenges posed by evolving scam tactics. The main limitations include data dependence, the need for continual updates, and the complexity of model explainability.

# 10. Lessons Learned

Throughout this project, we learned the importance of:
•	Data Preprocessing: Proper data cleaning and preprocessing are crucial for model performance.

•	Balanced Datasets: Ensuring a balanced dataset helps in training effective models.

•	Model Evaluation: Using various metrics provides a comprehensive understanding of model performance.

•	Adaptability: Models must be adaptable to evolving patterns in fraudulent behavior.

# Appendix

# Dataset Source

The dataset used in this project is publicly available and was sourced from [Real / Fake Job Posting Prediction (kaggle.com)]. Further details can be referenced in the appendix.

