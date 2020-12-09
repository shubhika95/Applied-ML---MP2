# Applied-ML

I have worked with logistic regression, KNN, naive bayes, decision tree and random forest.

Worked with 2 sets of database for handwritten digits: sklearn-load_digits and sklearn-openML

Toy dataset for all of the classifiers (or as much as possible-maybe 2 to draw some conclusion) --> couldnt get to import this. Anyways it was another step, thats all. For optional and creativity, we can present working of various classifiers on 2 datasets.

There is one more training file for openML dataset (but it was more than 25mb, so didnt upload here currently) --> this is for openML dataset, since it is huge set of data for handwritten digits, it was getting difficult to import, so tried a different method



MINI PROJECT 3

So, i have been working with the dataset. The preprocessing for this particular sample was something that i found very challenging.
I have prepared bits and pieces for the project. We just need to connect the dots.

Firstly: the three files called, Baseline Model with Multi-Layer Perceptrons.pynb , Simple Convolutional Neural Network for MNIST.ipynb and Larger Convolutional Neural Network for MNIST.ipynb, runs for different CNN and perceptrons for "original" MNIST datasets. And this works with a very good accuracy.
Next: For the preprocessing, we have images from MNIST datasets, "modified" to have multiple digits in one image. We need to crop that out, predict the number and assign them the class from 0 to 9, based on the digit and if no digit class is 10.
For this, i tried cropping without using opencv as told earlier (File: crop_images.ipynb). For which i couldnt draw a proper logic. But i still uploaded the document, as it might help to run the preprocessing for entire dataset, once we figure out the preprocessing for just one single image (File: single_cropping.ipynb).
For single_cropping i just used one image from the dataset, trying to crop all images from here. I have used opencv, to threshold and draw contours to deterine the ROI for each image. Its almost done, we need to play around a little bit with thresholding limit and find one which works best in all possible situation.My approach would be try and error here, but if you have a better idea, lets just try it. Once we can find ROI, we can crop it, determine how many digits are there, assign classes and do it for the entire dataset.
Once, the training image and labels and testing images are preprocessed we can directly use them in the CNN scripts, to determine accuracy. So this is where we need to use functions to preprocess at each step and pass them to CNN scripting.

Once we are able to load these "modified" MNIST dataset, and get good accuracy it wont be difficult to plot them for different epochs.


Related and similar projects that might help you (I have been taking hints from some these projects executed on various MNIST dataset):
1. https://github.com/tiff-wang/ModifiedMNIST
2. https://www.pyimagesearch.com/2017/02/13/recognizing-digits-with-opencv-and-python/
3. https://gsari.medium.com/digit-recognition-with-opencv-and-python-cbf962f7e2d0
4. https://www.kaggle.com/whizzkid/crop-images-using-bounding-box
