# CNN_Project

CNN for Sentence Classification (Naver Movie sentiment analysis)<br>
Train convolutional network for sentiment analysis. Based on "Convolutional Neural Networks for Sentence Classification" by Yoon Kim, [link](https://arxiv.org/pdf/1408.5882v2.pdf).

* language : python
* OS environment : macOS Catalina
* IDE : Jupyter Notebook

**How to use**<br>
**CNN modeling with mecab word2vec model**
1. clone repository to your local computer
2. recommend to convert file extension to .ipynb
3. recommend to execute in jupyter notebook or google colaboratory environment
4. you can use raw ratings.txt or ratings_train.txt and ratings_test.txt in 'prep for modeling' folder
5. make word2vec model first with tokenize_mecab_300dim_w_sw.py file in 'mecab_0.7993_val_accuracy_py' folder
6. make cnn model with word2vec model with CNN_word2vec_mecab300dim.py file in 'mecab_0.7993_val_accuracy_py' folder
7. you can use 'stopwords.xlsx' in 'prep for modeling' folder for removing stop words (in my case, there was no big difference in val_accuracy(not-removed:0.7993, removed:0.7984))

8. if you want to see my other trials for modeling with some tuning in word2vec dimension(200/300),base_tokenizer(mecab/okt) and stopwords removal(o/x), see other ipynb files<br>

**updated model**<br>
2020.08.10<br>
preprocessing train/test sentences with mecab ([click to see the code](https://github.com/jyshin0926/CNN-for-sentence-classification/blob/master/CNN_word2vec_mecab300_update.ipynb))<br>
val_accuracy : 0.8437 <br>
val_loss : 0.4047<br>

2020.08.11<br>
adding l2 regularization ([click to see the code](https://github.com/jyshin0926/CNN-for-sentence-classification/blob/master/CNN_word2vec_mecab300_update_0.8468.ipynb))<br>
val_accuracy : 0.8468 <br>
val_loss : 0.4815<br>

adding embedding weights with word2vec model ([click to see the code](https://github.com/jyshin0926/CNN-for-sentence-classification/blob/master/update_CNN_word2vec_mecab300_0.8539.ipynb))<br>
val_accuracy : 0.8539<br>
val_loss : 0.4464<br>

