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

[**3. GMM**](https://github.com/snehaNegi/MACHINE-LEARNING-HOT-TOPICS/blob/main/3.%20GMM)

DataSet used: speech_music_classification

A set of training and test examples of music and speech are provided.

**Our Task:**

a Generate spectrogram features - Use the log magnitude spectrogram as before witha 64 component magnitude FFT (NFFT). In this case, the spectrogram will havedimension 32 times the number of frames (using 25 ms with a shift of 10 ms).

b Train two GMM models with K-means initialization (for eachclass) separately eachwith 
(i) 2 mixtures with diagonal covariance, 
(ii) 2 mixtures with full covariance and(iii) 5-mixture components with diagonal/full covariancerespectively on this data.Plot the log-likelihood as a function of the EM iteration.

c Classify the test samples using the built classifiers and report the performance interms of error rate (percentage of mis-classified samples) on the text data.

d Discuss the impact on the performance for different number of mixture components,diagonal versus full covariance ?
