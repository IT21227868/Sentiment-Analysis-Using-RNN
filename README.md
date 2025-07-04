# Sentiment-Analysis-Using-RNN
Sentiment Analysis for Amazon Fine Food Reviews Using an RNN Model.<br/>
<br/>
In our project, which used the Amazon Fine Food Reviews dataset (https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews), I chose a Recurrent Neural Network (RNN) for 
sentiment analysis because RNNs are particularly suited for sequential data like text, where understanding word 
dependencies and contextual information is crucial. RNNs can maintain a hidden state across different time 
steps, making them excellent for capturing patterns in user reviews.
In Preprocessing and Optimization: To prepare the dataset, I tokenized the reviews, reduced the vocabulary to 
10000 words, and padded the sequences to ensure uniform input lengths. This reduces the model's complexity 
and ensures faster computation while preserving important data patterns.
Model Architecture: The RNN model I built starts with an embedding layer, which converts words into dense 
vectors, capturing their semantic meaning. This is followed by an RNN layer with 128 units, where it processes 
each word sequentially. By leveraging RNN’s inherent ability to store contextual information, the model captures 
sentiment from the review texts. Additionally, I used Dropout layers with a rate of 0.5 to prevent overfitting by 
randomly deactivating neurons during training.
Training and Optimization: The model was trained using the Adam optimizer for faster convergence. To ensure 
efficiency, I employed Early Stopping to halt training when there was no significant improvement in the validation 
loss, thus preventing overfitting and unnecessary computations. After training for 5 epochs, the model achieved 
strong performance, with an accuracy of over 93%.
Performance Evaluation: The model performs sentiment classification with an accuracy of 93.72%. It achieves a 
precision of 95%, a recall of 97%, and an F1 score of 96% for positive sentiment classification, showing its strong 
ability to correctly predict positive reviews. The inference time of just 35ms ensures that the model can be used 
effectively for real-time applications.
In conclusion, the RNN model efficiently captures the sentiment in text reviews, providing useful insights for 
customer sentiment analysis.
