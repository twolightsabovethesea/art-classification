# Van Gogh or No?

Determining if images of artwork by Vincent Van Gogh or art _inspired_ by Van Gogh can be predicted by using machine learning.
---
![Image](https://vangoghornot.s3.amazonaws.com/van_gogh_resized/gogh10.jpg)

---
## Introduction
In this project we used machine learning to determine if Van Gogh paintings were done by the artist or were done by a child. 

## System Requirements
* AWS S3 -- used for storage of images
* Google Colab -- used to run Tensor Flow model
* HTML -- Website 
* Bootstrap -- website elements
* Jupyter Lab -- Data Storage

## Data Sources
* [Van Gogh Website](https://www.vincentvangogh.org/)
* Guthrie Memorial Library Facebook Page Hanover, PA 


## Van Gogh Website Created for Project
[Git Hub Pages](https://twolightsabovethesea.github.io/art-classification/)

## Project Description
This project used paintings by Vincent van Gogh to determine if the the image was done by the artist himself, or done by a child. Multiple machine learning models were used to test loss and accuracy. 
* Non-Convolutional Model - We used a nueral network model that did not use any convolutional layers within Tensor Flow. This model easily predicted the Van Gogh paintings giving us a score of 100%. Having an accuracy score that high is an indicator that something is not right. Adding more images, resizing those images, and created extra versions of those images for the model by using image manipulation to rotate and change contrast, resulted in an accuracy score of 74%, with a loss of 68%. Not satisfied with those results, we switched to a convolutional model.
* Convolutional Model - This model was developed using a combination of convolutional layers and dense layers in conjuction with maximum pooling and flattening to predict the images. The accuracy and loss of this model was improved by adding more Van Gogh paintings to the sample size. The addition of these additional paintings resulted in the model's accuracy score increasing and loss decreasing. The accuracy score was [SCORE] and the loss was [SCORE]. Initially when we tried to work with this model, the limitations of Google Colab and our indiviual computers did not allow it to run.  If we had access to more robust cloud computing, that would have been the optimal solution. However, we were able to run the model on a single computer under different conditions.

## Conclusion
After testing the two model types we found that once trained using a convolutional model, our machine learned to differentiate between a Van Gogh painting and that of a similar piece of work done by a child. While we found limitations in our models, we discovered that it is quite impressive that a machine can make predictions regarding images without being able to "see". Given the time alloted, we created a model that was robust in predicting a Van Gogh painting, but there was a limitation in predicting if the image used was *not* a Van Gogh. In conclusion, we found that the best predictor of art is the human eye.


