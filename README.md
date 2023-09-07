# Arabic-dialect-Identification

 ![Logo](https://github.com/iRaneem/Recipes-Generator/blob/main/logo.jpg)
 
   we aim to provide a framework for understanding the linguistic and cultural diversity of the Arabic-speaking world and to help scholars and researchers analyze and compare these dialects. So we developed a model that takes a text as an input and gives you the name of the dialect as an output.


We used 3 models to get the best results:
- Multinomial Naive Bayes NB
- Support Vector Classification SVC
- Fully Connected Neural network model using the Keras library

# Design 💻
  collect a labeled dataset of tweets in various Arabic dialects.
Preprocess the dataset by tokenization, removing URLs, mentions, hashtags,
and stop words, and performing stemming/lemma.
Split the dataset into training and testing sets.
Choose a suitable model architecture, such as a Naive Bayes and LinearSVC
classifier and neural network.
fine-tune the model using Grid Search.
Evaluate the model on the testing set to measure its performance.
Deploy the model to make real-time dialectal Arabic predictions for user input
texts

# OBSERVATION
  First, we trained Multinomial Naive Bayes which gave us 0.3 accuracy which was considered very
low. We tried to overcome that by reducing the class number from 18 classes at the country-level
delicate to 6 classes at the regional level. By doing so we increased accuracy up to 0.69, which is
still unreliable.

  Another solution is to change the model. We trained a linear SVM model to increase the accuracy. In
the beginning, we observed 0.49 which is better than 0.3 of Multinomial NB. Then, we did regionlevel delicate classification which resulted in 0.68.
Finally, we designed a neural network and managed to increase the accuracy to 0.72
# CONCLUSION AND FUTURE WORK 🚀 
  In conclusion, Arabic delicate identification has emerged as an important research topic in recent
years. Several approaches have been proposed to address the challenges of Arabic delicate
identification, including machine learning algorithms, and natural language processing techniques.

  In the future, we want to focus on developing more effective algorithms for handling noisy and
unstructured data, exploring cultures that could be a promising avenue, and investigating the use
of alternative data sources such as speech and audio signals
