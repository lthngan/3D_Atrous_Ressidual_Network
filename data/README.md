# Overview
In recent years, Deep Neural Networks (DNNs) have achieved state-of-the-art performances in a variety of recognition and segmentation tasks in medical imaging. In this paper, we present a multi-task cascades network for both detecting and segmenting brain tumor. Our model consists of two networks, respectively differentiating brain tumor region and estimating brain tumor masks. These networks are formed as a cascaded structure, and are designed to share their feature maps. To effectively detect the brain tumor, our detection network processes contextual regions around ground-truth instances instead of processing every pixel. The proposed network is built on our novel backbone network architecture \textbf{3D atrous residual network}  which enables the gradient from the deep layer to be directly propagated to shallow layers and features of very different depth are preserved and used for refining each other. In order to incorporate larger context in volume MRI data, our network is designed with 3D atrous convolution which enlarges the field of view of filters. Our proposed network is evaluated on both BRATS 2015,  and BRATS2018 and compared against state-of-the-art approaches.

# Requirements
- A CUDA compatable GPU

- Tensorflow ( https://www.tensorflow.org/install/)

- NiftyNet(http://niftynet.readthedocs.io/en/dev/installation.html): pip install niftynet


- BraTS 2015, 2017, 2018 dataset http://braintumorsegmentation.org/
