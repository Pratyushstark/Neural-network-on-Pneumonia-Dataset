# Neural-network-on-Pneumonia-Dataset
The link to the dataset used in the project is https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia
ABOUT DATASET
We choosed the Pneumonia Dataset consisting of 1341 normal images of lungs and 3875 images of lungs having Pneumonia in the training data set. Followed by 234 normal images and 390 lungs having Pneumonia in test data set also it consists of validation data set of 16 images.
The main motive behind this project was to help the doctors in distinguishing between x-rays of a normal lungs and Pneumonia patient's with the help of deep-learning and AI.
The datasets are stored in Traingen, Testgen, Valgen directories. Followed by building few models to train the dataset on
Basic CNN architecture and as  we haven't done any class augmentation and the class datasets are highly imbalanced so the model validation accuracy is comparatively lower than training accuracy but the validation loss is higher than training loss.
Still The Auc is 0.904 which indicates that our vanilla model effectively distinguishes between normal and lungs with Pneumonia as well as there is a trade of between the precision and recall in the model. Also the confusion matrix gives us the clear picture about true and false predictions.
Once again the model was trained on the same weights with the expectations of getting any better outputs but it failed.
Saliency maps are used to visualize our model results such as grad cam and smooth gradcam to visualize our results.
In the last we used SOTA MobileNet and DenseNet and we observed that by using Transfer learning the validation accuracy is being improved if compared with the second model and it looks more promising in classying the images more accuartely. Since in the plots of Smooth Grad and Grad Cam for the case of Pneumonia we can observe that it not only detects if a person is having disease or not rather in Grad Cam it shows which parts of lungs are mostly affected due to the Pneumonia. 
This could be dployed in the future works as well as as a development we may try to implement CLAHE (Contrast Limited Adaptive Histogram Equalization) to get even more bettr results.
