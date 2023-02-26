# Yale-Face-Recognition
Principal Component Analysis (PCA) practice on [Yale Face Database B](http://cvc.cs.yale.edu/cvc/projects/yalefaces/yalefaces.html).

## Dataset Introduction
The Yale Face Database B consists of single light source images of 10 subjects, each seen in different poses and illumination conditions. In the provided form the database is divided into 5 subsets. In subset 0 the subject is illuminated by an almost frontal light source, while for subsets 1-4 the light source is gradually moved along the horizon. Subset 0 will serve as the training set, while subsets 1-4 are used for testing.

In the first part, we take pictures from subset 0 as the training set, whose labels are define as the person ID, and take pictures from other 4 subsets as test set. We change the amount of principal components used (from 1 to 20) to investigate its impact on recognition performance with KNN.

In the second part, we repeat the above experiment without using the first three principal components and investigate the recognition performance.

## File Description
* `data` : The default folder to save the modified version of the [Yale Face Database B](http://cvc.cs.yale.edu/cvc/projects/yalefaces/yalefaces.html)
* `face_recognition.ipynb` : A IPython Notebook to analyze database