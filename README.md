Email_Fraud_detection

Fraud Detection in Emails using Machine Learning

Overview  
This project focuses on detecting fraudulent emails using two machine learning models:  
Logistic Regression – A classification model that detects fraud based on word importance.  
Conditional Random Fields (CRF) – A sequence-based model that detects fraud by analyzing word relationships.  

 Models Implemented  
Logistic Regression  
A supervised learning algorithm used to classify emails as fraudulent or non-fraudulent. It converts text into numerical features using TF-IDF.

Evaluation Metrics  
 Precision – Proportion of correctly identified fraudulent emails.  
 Recall– Proportion of actual fraudulent emails correctly classified.  
F1-Score – Balances Precision and Recall.  
 ROC-AUC– Measures model’s ability to differentiate between classes.  

 Assumptions  
Each word in an email contributes independently to classification.  
The model does not consider the sequence of words, only their presence and importance.  

 Conditional Random Fields (CRF)  
CRF is used for sequence labeling tasks, such as Named Entity Recognition. It analyzes the relationships between words to detect fraudulent patterns.  
 Key Features  
Considers the order of words and surrounding context.  
Identifies key entities (e.g., names, organizations, locations) to detect fraud.  

 Assumptions  
 The sequence of words matters in detecting fraud.  
Context influences word classification.  
 Model Performance Comparison  

 Model Suitable for Strengths | Limitations 
|Logistic Regression | Text classification | Works well with large datasets and identifies fraudulent emails based on word importance | Ignores the sequence of words |
|CRF| Sequence labeling | Considers the order of words, making it ideal for entity-based fraud detection | More complex and computationally expensive |

Business Context  
When to Use Logistic Regression?**  
Best for detecting fraud using specific keywords (e.g., **"urgent transfer"**).  
Efficient when analyzing large datasets with individual word importance.  

When to Use CRF?
Best for detecting fraud based on word sequences(e.g., **"urgent" followed by "bank"**).  
Useful when entity recognition and context matter in fraud detection.  

Combining both modelscan improve fraud detection accuracy.  

Conclusion  
Logistic Regression is great for text-based fraud detection using word importance.  
CRF is powerful when detecting fraud using word sequences and context.  
A hybrid approach using both models may yield better fraud detection results.  

 Implement deep learning models(e.g., BERT, LSTMs) for better fraud detection accuracy.  


How to Run the Models  

bash
Install dependencies
pip install sklearn pandas numpy sklearn-crfsuite
