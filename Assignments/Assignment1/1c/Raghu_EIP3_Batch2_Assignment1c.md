# Raghu_Batch5_Assignment1
26/02/2019

## Topic 1: Convolution

Refers to combining 2 matrices to provide an output matrix. In neural networks image recognition and classification are carried out using Convolution technique.

Consider a grayscale (size 28 X 28 X 1) image showing a single digit number. Our aim is to identify the number. There are 10 possible results (0-9). Every pixel's intensity in the image is represented by a value.

![https://chrisjmccormick.files.wordpress.com/2015/01/layer_1.png](file:///C:/Users/rragh/AppData/Local/Temp/msohtmlclip1/01/clip_image002.png)

When a random 3X3 filter slides on this image to extract the features, it results a 26 X 26 output. Convoluting again results in 24 X 24 and so on till it reaches 10 X 10 where a well learnt neural network gives the expected output.

------------------------------------------------------------------------------------------------
## Topic 2: Filters / Kernels

Filters are matrices that convolve on an image, used for feature extraction. Consider a single digit number as follows:
 __
 __|
 __|

 We consider 2 **"filters"**  to pull out the features from this image. Horizontal dashes "-" and the vertical ones "|".  Convolution results in:

 Feature Map 1:
  __                        
  __     
  __


Feature Map 2:

|
|

Number of filters is equal to the number of feature maps obtain post convolution.

In CNN, at some point to compress the number of channels we reduce the number of filters and apply point convolution (1 X 1 filter) so as to optimize the model.

------------------------------------------------------------------------------------------------
### Topic 3: How to create an account on GitHub and upload a sample project

Git is a distributed version control system for source code maintenance. Following are the steps:

Create an account in  [GitHub](https://github.com/)

Install [GitSCM](https://git-scm.com/downloads)

    Initial settings..

![0.bh9snlp5q3.png](https://github.com/rraghu214/MLBLR/blob/master/IMG/0.bh9snlp5q3.png?raw=true)

    Create a new repo


![0.lo25v5pomud](https://github.com/rraghu214/MLBLR/blob/master/IMG/0.lo25v5pomud.png?raw=true)

    Once created, the next steps are intutive..


![0.qcboctw8fo](https://github.com/rraghu214/MLBLR/blob/master/IMG/0.qcboctw8fo.png?raw=true)

    Use "git init" to promote it to a git folder

![0.r3olhtpyvk7](https://github.com/rraghu214/MLBLR/blob/master/IMG/0.r3olhtpyvk7.png?raw=true)

    Add files to staging area, which is like a local versioning system.

![0.iwfi8nha2r](https://github.com/rraghu214/MLBLR/blob/master/IMG/0.iwfi8nha2r.png?raw=true)


    Commit changes to Staging area.

![0.szn82tq02pk](https://github.com/rraghu214/MLBLR/blob/master/IMG/0.szn82tq02pk.png?raw=true)

    Set remote repo URL for the code to be pushed to Git server.


![0.xg95h49pfah](https://github.com/rraghu214/MLBLR/blob/master/IMG/0.xg95h49pfah.png?raw=true)

     Push changes

![0.ccbg3a1mdb](https://github.com/rraghu214/MLBLR/blob/master/IMG/0.ccbg3a1mdb.png?raw=true)

     Verifying changes..

![0.pllarprggb](https://github.com/rraghu214/MLBLR/blob/master/IMG/0.pllarprggb.png?raw=true)

  Users can initialize this remote repository and checkout the code locally by using **"git checkout <*****branch_name*****>"** and commit the same way!



----------------

### Topic 4: Epochs

Epochs are the number of times a neural network sees the entire training examples in a dataset. It consists of one forward propagation and one backward propagation. If you want to teach a network to recognize the letters of the alphabet, 100 epochs would mean 2600 individual training trials. We don’t pass the entire dataset for training, but divide them into batches. If batch size is 50, it takes 52 iterations to complete one epoch.



-------------------

### Topic 5: Receptive field

The receptive field in a convolutional neural network refers to the part of the image that is visible to one filter at a time. This receptive field increases linearly as we stack more convolutional layers.



![](https://cdn-images-1.medium.com/max/1600/1*J-SPK7qCnLdYUE00RMTw-A.png)

---------------

In the above diagram, the right most layer has 5X5 global receptive field and 3X3 local receptive field. Local receptive field is the visibility of a neuron to its immediate preceding layer.

----------

