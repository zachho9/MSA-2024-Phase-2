Applied Convolutional Neural Network (CNN) and Vision Transformers (ViT) on given dataset:
* **CNN**:
    * Loaded train, val, test data set into working folder.
    * Processed datasets for modeling.
    * Created CNN network and fed in train set.
    * Predicted on val and test sets.
    * Accuracy on val set: about 0.846 (might change slightly after re-run).
    * Despite the accuracy was not bad, looking at the confusion matrix, the majority of the images were classified incorrectly. For example, 63/500 label 4 images were identified as label 8, only 45/500 were correctly classified, indicating bad performance of the current model.
    * Needed more hyperparameter tuning for better results, but it would consume lots of time and resources.
* **ViT**: 
    * Loaded train, val, test in input folder.
    * Processed images for modeling.
    * Created ViT model and fed in train set.
    * Predicted on val and test sets.
    * Accuracy on val set: about 0.918 (might change slightly after re-run).
    * According to the confusion matrix, the majority of the images were correctly classified, indicating good performance of the model.
    * ViT required fewer hyperparameter tuning than CNN.

Thus, Chose ViT for final output.