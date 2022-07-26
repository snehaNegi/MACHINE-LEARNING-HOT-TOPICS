# MACHINE-LEARNING-HOT-TOPICS

[**1.PCA and LDA implementation**](https://github.com/snehaNegi/MACHINE-LEARNING-HOT-TOPICS/blob/main/PCA%20and%20LDA%20implementation.ipynb) 


DataSet used: emotion_classification

**Our Task:**
15 subject faces with happy/sad emotion are provided in the data. Each image is of
100x100 matrix. Perform PCA on to reduce the dimension from 10000 to K (using
PCA for high dimensional data) and then perform LDA to one dimension. Plot the one
dimension features for each image. Select the optimum threshold to classify the emotion
and report the classification accuracy on the test data. What is the best choice of K
which gives the maximum separability ?



[**2. Speech Spectogram**](https://github.com/snehaNegi/MACHINE-LEARNING-HOT-TOPICS/blob/main/2.Speech%20Spectogram.ipynb)

DataSet used: speech


**Our Task:**

The files are in wav format sampled at 16kHz. Write a function to compute the spectrogram of clean and noisy files (use 25 ms Hamming window with a shift of 10 ms, compute 256 point magnitude FFT and retain the first 128 dimensions in each window, apply log of the magnitude of the FFT.). 

For example, a speech file of 3s will have a spectrogram of
size 128×298 (without any padding at the end, where 128 is the dimension of the feature
vector and 298 is the number of frames).

(a) Assume that each speech frame (128 dimensional vector) is independent of each other.
From the clean files, compute the whitening transform. Apply the transform on the
noisy speech features. Find the average of the absolute value of the non-diagonal
entries of the sampled covariance matrix of the “whitenned” clean and noisy speech
features. Comment on use of whitenning when the data distribution has changed.
(b) Repeat the above procedure by reversing the roles of clean and noisy files.

[**3. GMM**](https://github.com/snehaNegi/MACHINE-LEARNING-HOT-TOPICS/blob/main/3.%20GMM.ipynb)

DataSet used: speech_music_classification

A set of training and test examples of music and speech are provided.

**Our Task:**

a Generate spectrogram features - Use the log magnitude spectrogram as before with a 64 component magnitude FFT (NFFT). In this case, the spectrogram will have dimension 32 times the number of frames (using 25 ms with a shift of 10 ms).

b Train two GMM models with K-means initialization (for eachclass) separately each with 

(i) 2 mixtures with diagonal covariance, 

(ii) 2 mixtures with full covariance and

(iii) 5-mixture components with diagonal/full covariancerespectively on this data.Plot the log-likelihood as a function of the EM iteration.

c Classify the test samples using the built classifiers and report the performance interms of error rate (percentage of mis-classified samples) on the text data.

d Discuss the impact on the performance for different number of mixture components,diagonal versus full covariance ?

[**4. Logistic Regression & regularisation**](https://github.com/snehaNegi/MACHINE-LEARNING-HOT-TOPICS/blob/main/Logistic%20Regression%20with%20regularisation)

DataSet used: movieReviews1000.txt

**Our Task:**

a. Split the data into two subsets. One for training (first 3000reviews) and the otherfor testing (last 1000 reviews).

b. Use TF-IDF features and train PCA (using the training data)to reduce the data to30 dimensions.

c. Split the training data randomly into set of 2500 for model training and 500 forvalidation. 
Train a logistic regression model.  Implement the stochastic gradientdescent algorithm by hand without using any tools.
Show the loss value for each epoch on the training and validation dataset (for 20 epochs). 

Test on the test data and report the performance in terms of review classificationaccuracy.
Compare there performance for different choices - batch size [32,64,128],learning rate [1e-3,1e-2,1e-1]. Show the loss curves for each case.d Implement the logistic regression with L2 weight regularization. 
Show the losscurves for regularization coefficient value of 1e−2, 1e−1 and 1. Do you see anyoverfitting/under-fitting for any of these choices. 
Test on the test data and reportthe performance on the test set in terms of review classification accuracy.



