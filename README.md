# Text Classification
- This project is designed to showcase the implementation of a Machine learning (NLP) models for classify the text.
## ***Project Overview***
### The project consists of three main components:
#### a. Spell Checker
#### b. EDA
#### c. Modeling
## ***Technologies Used***
- Numpy, Pandas
- Tensorflow, Keras, sklearn
- tashaphyne
- CNN 
## ***TASK 1***
- Time complexity: O(n) if word exist and o(k*m) if will get the 4 similar words.
where k:  is the number of elements in the word, and m: the maximum length of words in the list
- Space complexity: O(n) to store the dictionary in a hash table or a tree data structure and O(1) for other operations like add word
## ***TASK 2 & 3***
- The model for this task is a conv1D model with maxpooling and dropout to avoid the overfitting 
- I prefered to use conv1D over the RNN model to make the task faster and the data is not too big so if i used a complex model it will overfit and will take lots of time in training
## ***Evaluation***
![Model](https://github.com/osamashaaban/Text-Classification/assets/63675685/81e23033-3a2c-4177-b5c5-375babb1a33b)
- I used the F1 score, Precision and Recall for evaluating the model F1 as it is the harmonic mean of precision and recall, and provides a single value that balances both metrics.
- Precision gives an insight about how good does the model in the data he tested so if it gives 50% it means that the model could predict 50% of the data correctly"من كل الداتا الي حاول يتوقها كام واحده توقعها صح"
- Recall is about how much the model could predict correctly from the actual true data.
  ![Precisionrecall svg](https://github.com/osamashaaban/Text-Classification/assets/63675685/224a362e-ad15-4b47-818e-b2b2931395f7)


## ***Future Problems***
- I tried trained the model on only the files of stories as i though that is the most relevent sentences to the topic not the comments on every post and actually i found that the data is balaced but small. so I guess if the comments are pure relevent to the topic of the story it may help to enhace the metrics of the model
- I found that the classical ML models couldn't catch patterns between the data well so that I decided to use moder ML. when I tried to use dequecial models it took lots of time and the model overfits the data, so that I decided to use something in between. which is the CNN as it is fast and may enhace the accuracy and it did it very well copared to other models but still needs some enhancements
- I think if we could find more data and try not to take all the senteces length so that the model avoid the overfitting and the fanishing of the gradients it will works well. in additoin to using a suitable architecture or using Transfer learning with big and powerful models it will help alot but it will affect the size of the model and will need more resources for training
## ***Note***
- The process of tokenization and padding was very heavy on the colab resources so that I tried to get more resources up to 25 GB RAM to complete the processes of embedding and training and that while using only files of stories.
- this happened because of the length of the data that needs to be tokenized and padded for the model and that's why I think taking only a specific lenght from the text will help the model to work better

