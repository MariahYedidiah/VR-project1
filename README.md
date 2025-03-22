OBJECTIVE:---To conpare performances of different traditional classifiers including neural network and CNN--and show CNN outperforms them all.

DATASET:--the dataset was initially a folder,which was zipped to upload to goggle colab and then unzipped from there,it has 2 subfolders with_mask and without_mask of images with masked and without mask images respectively,in jpg and png formats.



CONCLUSION:--

For feature extraction ,once plain flattening and once hog was used,hog showed better performance .
The chosen models are Random forests with 100 decision trees,Svm,and 3 layers Neural n/w(with 1 hidden layer)effectively handle high-dimensional data and mitigate the impact of irrelevant features. Since this is a supervised learning task, KNN and GMM were not considered. Logistic regression,being a linear classifier, was not included. Traditional ML methods, such as SVM and random forests, showed varying results, with SVM performing better. As expected, the neural network outperformed traditional models, leveraging its ability to learn hierarchical representations.On using HOG feature extraction,the accuracy further improved for the traditionalo methods as expected,but CNN still outperforms the traditional methods ,including Neural network of 3 layers(1 hidden),that was used(an  attempt to use a 6 layer Neural network showed overfitting,with 0 train loss and very high test losses.)For sift we have tried using a 5 layer neural network and it has shown lower performance as compared to 3 layer hog nn.
To do SIFT , the SIFT descriptors for the  images have variable lengths (since different images yield a different number of keypoints), so when we tried to create a NumPy array, the elements were of different sizes.

A simple fix is to convert the descriptors for each image into a fixed-length feature vector by taking the mean of all descriptors for that image. This way, regardless of how many keypoints are detected, we got a 128-dimensional vector (since each SIFT descriptor is of length 128).

HOW TO RUN:-
To run each part of code,the zipped file dataset.zip is to be loaded when asked 
