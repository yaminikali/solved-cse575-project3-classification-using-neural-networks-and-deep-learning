Download Link: https://assignmentchef.com/product/solved-cse575-project3-classification-using-neural-networks-and-deep-learning
<br>
In this part, we will revisit the Handwritten Digits Recognition task in Part 1, using a convolutional neural network. The basic dataset is the same MNIST dataset from Part I,

but you may choose to use only a subset for training and testing, if speed performance with the entire dataset becomes a bottleneck. For example, you may use only 6000 samples for training (each digit with 600 samples) and 1000 samples for testing (each digit with 100 samples).

The basic requirement of this part is to experiment with a convolutional neural network with the following parameter settings:

<ul>

 <li>The input size is the size of the image (28×28).</li>

 <li>The first hidden layer is a convolutional layer, with 6 feature maps. The convolutionkernels are of 3×3 in size. Use stride 1 for convolution.</li>

 <li>The convolutional layer is followed by a max pooling layer. The pooling is 2×2 with stride 1.</li>

 <li>After max pooling, the layer is connected to the next convolutional layer, with 16 feature maps. Theconvolution kernels are of 3×3 in size. Use stride 1 for convolution.</li>

 <li>The second convolutional layer is followed by a max pooling layer. The pooling is 2×2 with stride 1.</li>

 <li>After max pooling, the layer is fully connected to the next hidden layer with 120 nodes and relu as theactivation function.</li>

 <li>The fully connected layer is followed by another fully connected layer with 84 nodes and relu as theactivation function, then connected to a softmax layer with 10 output nodes (corresponding to the 10 classes).</li>

</ul>

We will train such a network with the training set and then test it on the testing set.

You are required to plot the training error and the testing error as a function of the learning epochs.  You are also required to change some of the hyper-parameters (the kernel size, the number of feature maps, etc), and then repeat the experiment and plot training and testing errors under the new setting. These are the minimum requirements. Additional requirements may be added (like

experimenting with different kernel sizes, number of feature maps, ways of doing pooling, or even introducing drop-out in training, etc.).

Algorithm:

Convolutional Neural Network

Resources:

MNIST dataset, Google CoLab

Workspace:

Google CoLab (see file intro_to_colab.docx for more details)

Software:

Google CoLab

Language(s):

Python

Getting Started:

Read this document carefully, as well as  additional files included (intro_to_colab.docx and<a href="https://asu.instructure.com/courses/31489/files/10486250/download?wrap=1"><strong> baseline.docx</strong></a> ). For more details about Colab, please go to

<a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>https://colab.research.</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>g</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>oo</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>g</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>le.com/notebooks/welcome.ip</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>y</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>nb</strong></a>

<a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>(https://colab.research.</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>g</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>oo</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>g</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>le.com/notebooks/welcome.ip</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>y</strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"><strong>nb) </strong></a><a href="https://colab.research.google.com/notebooks/welcome.ipynb"> </a>

Required Tasks:

<ol>

 <li>Read <a href="https://asu.instructure.com/courses/31489/files/10217264/download?wrap=1"><strong>docx</strong></a> to get familiar with the platform.</li>

 <li>Run the baseline code (<a href="https://asu.instructure.com/courses/31489/files/10486250/download?wrap=1"><strong>docx</strong></a> ) and report the accuracy.</li>

 <li>Change the kernel size to 5*5, redo the experiment, plot the learning errors along with the epoch, andreport the testing error and accuracy on the test set.</li>

 <li>Change the number of the feature maps in the first and second convolutional layers, redo theexperiment, plot the learning errors along with the epoch, and report the testing error and accuracy on the test set.</li>

 <li>Submit a brief report summarizing the above results, along with your code.</li>

</ol>

Optional Tasks:

<ol>

 <li>Change the kernel size to 9*9 and redo the experiment and report your results.</li>

 <li><a href="https://keras.io/optimizers/">Use another optimizer (it can be chosen from</a><a href="https://keras.io/optimizers/"><strong> https://keras.io/optimizers/</strong></a></li>

</ol>

<a href="https://keras.io/optimizers/"><strong>(https://keras.io/optimizers/) </strong></a><a href="https://keras.io/optimizers/">) and at least 3 different learning rate to redo the expe</a>riment, and report the accuracy vs learning rate on the test set.

<ol start="3">

 <li>Use average pooling and redo the experiment an0d report your results.</li>

</ol>

Optional tasks are to be explored on your own if you are interested and have extra time for them. No submission is required on the optional tasks. No grading will be done even if you submit any work on the optional tasks. No credit will be assigned to them even if you submit them. (So, please do not submit any work on optional tasks.)