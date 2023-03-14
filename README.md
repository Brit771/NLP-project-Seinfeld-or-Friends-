# NLP project - Seinfeld or Friends

![cc!](https://github.com/Brit771/NLP-project-Seinfeld-or-Friends-/blob/main/assets/Friends-vs-Seinfeld-Rivalry.JPG?raw=true)

In this project I was given a dataset containing the scripts of all Seinfeld and Friends episodes.
my goal is to create a deep learning model that could identify whether a line was taken from a Seinfeld episode or a Friends episode.

More info down below.

* [Data]()
* [The model]()
* [Results]()

## Data
The dataset contains total of 70405 scripts of Seinfeld and friends episodes.
* 39092 Friends Samples
* 31313 Seinfeld Samples

#### Preprocessing
Below are some of the operations I performed to clean the data:
* Converting all letters to lowercase
* Removing special characters,newline characters and stopwords

In addition I was Stemming the text.

Then I did Train-test-valdiation split , tokenizing using Keras' tokenizer and Converted to sequences.

## The model

I used a fully connected 1D CNN model with an embedding layer and a dropout between the layers.
In the FC layers I used the Relu activation function and in the last layer I used the sigmoid  activation function for the classification.

| subject  | description |
| ------------- | ------------- |
| epochs number| 5 | 
| batch size |64 | 
| Optimizer | adam | 
| evaluation metric | Accuracy | 

## Results

The accuracy score - 0.8118

### evaluate per actor:

| Actore  | Accuracy Score |
| ------------- | ------------- |
| joey| 0.7 | 
| phoebe | 0.697 | 
| elaine | 0.472 | 
| chandler | 0.69 | 
| kramer |  0.439 | 
| monica | 0.6727 | 
| ross | 0.7157 | 
| george | 0.411 | 
| rachel | 0.722 | 
| jerry | 0.417 | 

We can see that joey,phoebe and rachel have the highest accuracy score. And george, kramer and jerry got the lowest accuracy scores.

![ps!](https://github.com/Brit771/NLP-project-Seinfeld-or-Friends-/blob/main/assets/Phoebe%20Shocked.gif)

## Vizualization

Let's see what a Friends Dialogue looks like using a word cloud:

![f!](https://github.com/Brit771/NLP-project-Seinfeld-or-Friends-/blob/main/assets/Friends%20Dialogue.JPG)

![s!](https://github.com/Brit771/NLP-project-Seinfeld-or-Friends-/blob/main/assets/Seinfeld%20Dialogue.JPG)








* 




