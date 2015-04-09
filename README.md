# TFT Miniature Billboard
A patch to use with a 2.4” TFT screen and an arduino microcontroller to
display digital adverts, like on a digital billboard.

For a complete tutorial, see my blog post at http://apheleia.me/how-to-create-a-miniature-billboard/

## Setup
Two constants are set at the top of the patch for setting up your project.
```C
// DELAY defines the delay in between consecutive images in milliseconds.
#define DELAY 3000
// IMAGE_COUNT defines the number of image files on the micro SD card.
#define IMAGE_COUNT 4
```

## Images
All images have to be 24-bit BMP images (they _have_ to be 24 bits).
You have to put the images you want to use in the root directory of the micro SD card.
They need to be numbered using two digits, starting at one and up to the number of configured images (see IMAGE_COUNT above).
For example:
```
01.bmp
02.bmp
03.bmp
04.bmp
```
Thus you can have a maximum of 99 images.

## Appreciations

Graphics/images from:
* http://fsfe.org

Original code from:
* https://github.com/adafruit/TFTLCD-Library
* https://github.com/Smoke-And-Wires/TFT-Shield-Example-Code
