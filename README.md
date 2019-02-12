# TTA-Keras

Test-Time Augmentation is a very efficient way to improve the results of your model at **testing** time.


Here is how it works for a single image:

After having trained our network, we can show it a test image and see it prediction.

Here is the query image :

![Optional Text](../master/Images/test_image.png)

Its prediction is :

![Optional Text](../master/Images/test_pred.png) 

While the true label is : 

![Optional Text](../master/Images/test_label.png)

So the test image is misclassified.

But what happens if we apply TTA to that image ? Meaning that we will show the model several slightly modified versions of the image and average its predictions.

The 5 modified images are : 

![Optional Text](../master/Images/tta_images.png)

And the corresponding predictions : 

![Optional Text](../master/Images/tta_pred1.png)

![Optional Text](../master/Images/tta_pred2.png)
![Optional Text](../master/Images/tta_pred3.png)
![Optional Text](../master/Images/tta_pred4.png)
![Optional Text](../master/Images/tta_pred5.png)


By now taking the average we have:
![Optional Text](../master/Images/tta_avg_pred.png)

And the image is correctly classified ! 



This notebook shows how to use it with Keras


Further explanation can be found [here](https://towardsdatascience.com/test-time-augmentation-tta-and-how-to-perform-it-with-keras-4ac19b67fb4d)
