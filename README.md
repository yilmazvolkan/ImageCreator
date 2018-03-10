# ImageCreator
Image Creation app on Python via GAN

<p align="center">
<a href = "https://github.com/yilmazvolkan/ImageCreator"><img 
<img src="https://github.com/yilmazvolkan/ImageCreator/blob/master/Res/ai_art_logo.png" width="250" height="250"></a>
</p>
<p align="center">
    <a href="https://github.com/yilmazvolkan/ImageCreator/blob/master/README.md">
        <img src="https://img.shields.io/badge/DESCRIPTION-ONLINE-fb6a61.svg"
             alt="Description">
    </a>
    <a href="https://github.com/yilmazvolkan/ImageCreator/blob/master/Res/image_creator.py">
        <img src="https://img.shields.io/badge/Python-ONLINE-fa3b30.svg"
             alt="Python">
    </a>
    <a href="https://github.com/yilmazvolkan/ImageCreator/issues">
        <img src="https://img.shields.io/badge/ISSUES 3-CLOSED-f11306.svg"
             alt="Issues">
    </a>
</p>

## :flashlight: Before You Go

You need to install openCV library on Python. You can reach this library clicking on this [link](https://github.com/opencv/opencv).

## :tophat: Introduction

Neural networks are generally good at predicting or classifying things and solving problems. Howewer, scientists also want to create a type of neural network that can create for itself. Generative Adversarial Networks(GAN) can be used for generating images, image modification, super resolution, photo realistic images, speech generation, and face ageing.


GAN can actually generate images that they are not existed before. GAN consist of generator and discriminator components. Basically, generator creates images, and the discriminator assesses these images, then tells the generator whether those images are likely to be similar to real examples.


How do GAN work? Generator takes noise signal as input and creates random images. Since we want to train discriminator to make it smarter, we give additional real images. Then, it will give some probabilities with respect to real image. We take these values and look at what they should be. Resulting error backpropagated to discriminator and weights are updated in order to get more relevant images.


For the second time, discriminator takes new generated images as input without real images. Since the way the generator learns by trying to trick the discriminator and based on it will succeds or not it will update its weights in order to produce similar images. We take these values and look at what they should be. The error backpropagated to generator this time and weights are updated in order to create more relevant images.


These processes can be implemented on Python with the help of nn.Module class. We can simply implement generator and discriminator one by one and update weights according to resulting error. As an input we can give an image consists of small images. The training and creation of images takes approximately a day and at the end of each epoch we get an output image. At the beginning of process, these images are not seem to like anything since the training is not completed enough. However, while the program is running, we can see coming more relevant images. We can see the result below;

<p align="center">
<a href = "https://github.com/yilmazvolkan/FaceDetector/blob/master/Res/integral_image_calc.png"><img 
<img src="https://github.com/yilmazvolkan/FaceDetector/blob/master/Res/integral_image_calc.png" width="350" height="210"></a>
</p>


The results show us the algorithm learns how to use pixels and creates good images rather than some blur and ambiguous images.

## :blue_book: Readings

You can reach more information about object detection using a boosted cascade of simple features article by clicking on this [link](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.10.6807&rep=rep1&type=pdf).

Another good article about boosting image retrieval is accesible by clicking on this [link](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.136.2419&rep=rep1&type=pdf).


## :beers: Contributers


<p align="left">
<a href = "https://github.com/yilmazvolkan"><img 
<img src="https://avatars2.githubusercontent.com/u/28186366?s=400&v=4" width="120" height="120"></a>
</p>
