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

It's good enough for a picture with humans though!

All you have to do to get started is:
1 Install tensorflow if you don't have it yet(PixelLib supports tensorflow 2.0 and above)
pip install tensorflow

2 Install PixelLib
pip install pixellib (https://pypi.org/project/pixellib/)


