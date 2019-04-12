# Neural-Style-Transfer
This project applies a Neural Style Transfer algorithm to create images copying the content from a picture and the style from another picture.

The algorithm is composed of several main functions:
- 'content cost' function computing the cost (difference) between the generated image and the image from which the content needs to be copied
- 'style cost' computing the cost (difference) between the generated image and the image from which the style needs to be copied
- 'total cost' computing the weighted sum of the previous two

An optimisation algorithm iterates updating the pixels in order to minimise the total cost.

The algorithm is based on a pretrained VGG-19 convolutional neural network that, given its size, has not been included in the repo but can be downloaded from https://www.kaggle.com/teksab/imagenetvggverydeep19mat and should be unzipped and saved in folder named 'pretrained-model' to be located in the root repo.

The full code can be found in the Jupyter notebook 'full_code.pynb', while a brief report summarising the methodology and the results can be found in 'report.html'. The folder 'images' contains all the images used to realise the proposed examples, while the folder 'output' proposes all the generated images.
