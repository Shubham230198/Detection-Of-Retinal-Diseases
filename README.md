# Retinal-OCT-Images
To detect Retinal Diseases from medical X-ray images.

<h2> Description </h2>

The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (NORMAL,CNV,DME,DRUSEN). There are 84,495 X-Ray images (JPEG) and 4 categories (NORMAL,CNV,DME,DRUSEN).


<h2> Source / useful links </h2>

DataSource : https://www.kaggle.com/paultimothymooney/kermany2018 <br>


<h3> Type of Machine Learning Problem</h3>

<p> It is a one class classification problem, for a given image we need to predict if they are suffering from which disease. </p>

<h3> Performance Metric </h3>

Metric(s): 
* Precision Matrix
* Confusion Matrix

<h3> How does it work ? </h3>
* Understanding image data
* Image augmentation
* Applying model

<h3> Conclusion </h3>
1. We applied image augmentation to this dataset.<br>
2. We applied three model - InceptionNet and ResNet, with Transfer Learning. <br>
3. We have taken the weight of every model which is trained on imagenet dataset, we have not freezed the layer because the retina dataset is different from imagenet dataset.<br>
4. We used confusion matrix because dataset is imbalanced and so accuracy score may not give good sence of result.<br>
5. By seeing the confusion matrix of both model we can say that inception net has best recall  than other model, precision is also good for inception net.
