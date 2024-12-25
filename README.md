# Hate Speech Detection in Telugu Language Using Transformer Models and Machine Learning

The rise of hate speech on social media poses significant risks to social harmony, mental health, and security, making accurate detection essential. This research focuses on hate speech detection in Telugu, one of the most widely spoken Dravidian languages. However, the variety of Telugu language and many dialects as well as cultural differences are the factors that might be a challenge to solve.

## Traditional Methods
* Traditional models like n-grams and Bag of Words (BoW) which were evaluated with multiple machine learning classifiers.
* Among them, Logistic Regression performed the best, achieving an accuracy of 0.66 for n-grams and 0.65 for BoW.
* SVM also showed consistent results with 0.64 accuracy in both approaches.
* Overall, n-grams outperformed BoW in capturing features for hate speech classification, highlighting its suitability for text categorization tasks.

## Transformer Models + Machine Learning
* Transformer models outperformed traditional methods significantly.
* MuRIL achieved the highest accuracy of 0.78, with LaBSE close behind at 0.76.
* However, when transformer embeddings were paired with machine learning classifiers, performance was slightly lower.
* For instance, MuRIL with XGBoost achieved an accuracy of 0.71.
* Analyzing the confusion matrix for XGBoost + MuRIL revealed a balanced distribution of false positives and false negatives, with 180 instances of hate speech and 175 non-hate speech correctly classified.
  
![image](https://github.com/user-attachments/assets/a71df987-51ab-437b-8b1d-ab2ba7981104)

## Ensemble Embeddings 
* Combining transformer embeddings further enhanced performance.
* BERT + MuRIL achieved an accuracy of 0.76, while DistilBERT + LaBSE reached the highest at 0.77.
* These results demonstrate the ability of ensemble embeddings to capture rich linguistic features. 

## Visualization 
* The t-SNE visualization of ensemble embeddings showed clear separation of hate speech and non-hate speech clusters, confirming the effectiveness of ensemble models in retaining semantic distinctions.
* These results show that advanced NLP techniques can be used for the detection of multilingual hate speech.
  
![image](https://github.com/user-attachments/assets/2e16826a-ae4c-48b9-a32f-7839751bdeb2)

## Conclusion 
* Compared to traditional machine learning models, transformer models like LaBSE and MuRIL show remarkable performance, achieving high accuracy and F1-scores of up to 0.79.
* These models effectively handle the unique linguistic challenges of the Telugu language.
* We also found that combining embeddings from multiple transformers with traditional classifiers significantly enhances detection accuracy, showcasing the potential of hybrid systems for moderating hate speech.
* The future work will be, extending these techniques to more low-resource languages, exploring domain-specific embeddings, and improving the real-time efficiency of hate speech detection systems.



