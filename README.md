# Background_Change_Image

This rep is about changing the background of any image with merely 4-5 lines of code. A library in Python called PixelLib, makes this happen! 

PixelLib is a library created to ensure easy integration of image segmentation in real life applications. PixelLib now supports a feature known as image tuning.

The key role of image segmentation is to remove the objects segmented from the image and place them in the new background created. This is done by producing a mask for the image and combining it with the modified background. We make use of deeplabv3+ model trained on pascalvoc dataset. The model supports 20 common object categories, which means you can change the background of these objects in images.

The model supports the following objects listed below:
person,bus,car,aeroplane, bicycle, ,motorbike,bird, boat, bottle,  cat, chair, cow, dinningtable, dog, horse pottedplant, sheep, sofa, train, tv

Background effects supported are:
1 Changing the background of an image with a picture
2 Assigning a distinct color to the background of an image.
3 Blurring the background of an image
4 Grayscaling the background of an image

(Ref: https://www.kdnuggets.com/2020/11/change-background-image-5-lines-code.html)

However, when I tried the library over a variety of images, it gave best results on human pictures. With pictures of dogs, buses etc., it manages to mask the object well i.e. select the main object of the image well, but tends to blend the colors of the image.

An example of this is given below:
The original image was:

![bus](https://user-images.githubusercontent.com/66153946/98776433-ea132080-2414-11eb-8416-c4388c3f63f0.jpg)

And the updated image formed is:

![new_bus](https://user-images.githubusercontent.com/66153946/98777159-3f036680-2416-11eb-9a49-774fa644d7c0.jpg)

It's good enough for a picture with humans though!

The original image was:

![brooklyn](https://user-images.githubusercontent.com/66153946/98777384-9f92a380-2416-11eb-9b2b-ef7bc2896a2b.jpg)

And the updated image turns out to be:

![new_brook](https://user-images.githubusercontent.com/66153946/98777401-a6b9b180-2416-11eb-8dd9-8de2908fff52.jpg)

All you have to do to get started is:

1 Install tensorflow if you don't have it yet(PixelLib supports tensorflow 2.0 and above)
pip install tensorflow

2 Install PixelLib
pip install pixellib (https://pypi.org/project/pixellib/)

3 Download the deeplabv3+ pascalvoc model from [here](https://github.com/ayoolaolafenwa/PixelLib/releases/download/1.1/deeplabv3_xception_tf_dim_ordering_tf_kernels.h5) 


