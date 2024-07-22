Applied Convolutional Neural Network (CNN) and Vision Transformers (ViT) on given dataset:
* **CNN**:
    * Loaded train, val, test data set into working folder.
    * Processed datasets for modeling.
    * Created CNN network and fed in train set.
    * Predicted on val and test sets.
    * Accuracy on val set: about 0.846 (might change slightly after re-run).
    * Despite the accuracy was not bad, looking at the confusion matrix, most of the values were close to 50 with highest at 65. It indicated that the model would not perform well on unseen data. The overall accuracy was expected to be around 60-70.
    * Needed more hyperparameter tuning for better results, but it would consume lots of time and resources.
* **ViT**: 
    * Loaded train, val, test in input folder.
    * Processed images for modeling.
    * Created ViT model and fed in train set.
    * Predicted on val and test sets.
    * Accuracy on val set: about 0.918 (might change slightly after re-run).
    * ViT required fewer hyperparameter tuning than CNN.

Thus, Chose ViT for final output.