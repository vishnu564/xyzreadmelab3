# Lab Task-3: Training and Visualizing Word Embeddings and Using them for Spelling Error Detection

In this lab task, I have trained and implemented word2vec and glove model.

### File architechure

The main directory consists of four directories
- word2vec (CBOW embedding)
- word2vec (skip-gram embedding)
- GloVe embedding
- CNN

### Word2vec(CBOW embedding)

- I have implemented CBOW embedding using gensim from the python library. For this I have loaded my training data into a variable and performed all the text preprocessing on the training dataset
- Next, I have tokenized all the sentences and removed the stopwords from the sentences 
- Then words are been tokenized and finally fed to the model
- model is created using the Word2vec function which is imported from the gensim.models
- This model has predicted two similar words of same context
- Visulisation plots (PCA and t-SNE) for most similar words as well as the complete embedding space are done

### Word2vec (skip-gram embedding)

- Skip-gram embedding is implemented using gensim. 
- Text-Preprocessing and tokenization is done for the training data.
- Then cleaned data is fed to the model.
- This model has predicted two similar words of same context
- Visulisation plots (PCA and t-SNE) for most similar words as well as the complete embedding space are done

### Glove Embedding
- For Glove Embedding I have loaded a pre-trained model 
- Made few prediction using that model
- Visulisation plots (PCA and t-SNE) for most similar words as well as the complete embedding space are done

### CNN

Spelling error detection using CNN:
It is an interaction of identification and of mistakenly spelled words in a content. In common language, it fundamentally examines the content and concentrates
contained in it. It at that point looks at each word to a rundown of effectively spelled words (a greater amount of like a word reference) and henceforth distinguishes
the incorrectly spelled words.
Usage - We have actualized a binary characterization model of CNN in which we have utilized a dataset which contains accurately spelled words alongside some
wrongly spelled words in the proportion of 10:1 (i.e., 10 right words for each wrongly spelled word).
At that point we have passed the embeddings of this dataset shaped into the neural organization which repeat through different ages where every age has a specific
exactness and misfortune esteem which is adjusted after each age to build the precision of the yield model.
Remarks – It can be implemented utilizing different calculations and utilizing different models like – CNN and RNN or LSTM. Utilizing GPU, it is a super quick cycle
and its precision is likewise acceptable after numerous iterations of the model.
