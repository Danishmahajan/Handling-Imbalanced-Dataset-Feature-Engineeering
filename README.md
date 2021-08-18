# Handling-Imbalanced-Dataset-Feature-Engineeering

* Imbalance means that the number of data points available for different the classes is different:
If there are two classes, then balanced data would mean 50% points for each of the class. For most machine learning techniques, little imbalance is not a problem. So, if there are 60% points for one class and 40% for the other class, it should not cause any significant performance degradation. Only when the class imbalance is high, e.g. 90% points for one class and 10% for the other, standard optimization criteria or performance measures may not be as effective and would need modification.

![image](https://user-images.githubusercontent.com/64760966/129844042-56698129-3ac8-4112-b0c5-618488c0b28a.png)


<hr>

### Problem with Imbalanced data:

Feeding imbalanced data to your classifier can make it biased in favor of the majority class, simply because it did not have enough data to learn about the minority.

Let us understand the technique used for creating balanced data sets.

### Oversampling:

This technique is used to modify the unequal data classes to create balanced data sets. When the quantity of data is insufficient, the oversampling method tries to balance by increment the size of rare samples.

A primary technique used in oversampling is SMOTE (Synthetic Minority Over-sampling Technique). In this technique, the minority class is over-sampled by producing synthetic examples rather than by over-sampling with replacement and for each minority class observation, it calculates the k nearest neighbours (k-NN). By doing this, we have an advantage of No loss of information and also mitigate over fitting caused by oversampling.

### Under sampling:

Unlike oversampling, this technique balances the imbalanced data set by reducing the size of the class which is in abundance. There are various methods for classification problems such as Cluster Centroids and Tomek Links. The cluster centroid methods replace the cluster of samples by the cluster centroid of a K-means algorithm and the Tomek link method removes unwanted overlap between classes until all minimally distanced nearest neighbours are of the same class.By doing this, we have an advantage like Run-time can be improved by decreasing the amount of training data set and also helps in solving the memory problems

Balancing the imbalanced data is very important in ML in order to achieve the right accuracy . It is not 99% accuracy of the model that matter but the right accuracy of the model matters. There are many more techniques used to balanced the imbalanced data . But SMOTE is the one of the common technique used .
