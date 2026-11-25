# Recorded results

| File | Source | Scope and units |
|---|---|---|
| [Traditional sweep](sift_bow_svm_results.csv) | Supplied final results file, whose contents are comma-delimited text, copied byte for byte | 72 instance-classification configurations, stratified 80:20 split. `accuracy` is test accuracy; both accuracy columns are proportions. `avg_keypoints` is the mean count per image. |
| [Traditional notebook sweep](sift_bow_svm_notebook_70_30.csv) | Saved text output of the traditional notebook’s parameter-grid cell | 72 instance-classification configurations, stratified 70:30 split. Test accuracy is a proportion and SVM elapsed time is in seconds, both at printed precision. |
| [CustomCNN training](cnn_training_results.csv) | Saved output of the CustomCNN Adam training cell | Ten epoch records. Test accuracy in percent at the precision printed in the notebook. Training loss was unavailable in the saved text. |
| [CustomCNN grid](cnn_hyperparameter_results.csv) | Saved output of the CustomCNN hyperparameter cell | Eight settings and five epochs per setting. Loss is the recorded mean of training-batch cross-entropy losses. Test accuracy is in percent. Values retain printed precision. |

Both CNN files use the 51-class, 48,000-training and 12,000-test image configuration. The ResNet-18 outputs remain in the notebook. Category-grouped recall remains available as the [original figure](../docs/04_experimental_results.md).
