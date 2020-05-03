# Image Stitching

This repository contains an implementation of multiple image stitching.

So what is image stitching? In simple terms, for an input group of images, the output is a composite image such that it is a culmination of scenes. At the same time, the logical flow between the images must be preserved.

## Input images:
![Input image] (https://github.com/najma510/DeepPixel/blob/master/deeppixel/image_stitching_2/input/images/room1.jpg?raw=true)
![Input image] (https://github.com/najma510/DeepPixel/blob/master/deeppixel/image_stitching_2/input/images/room2.jpg?raw=true)
![Input image] (https://github.com/najma510/DeepPixel/blob/master/deeppixel/image_stitching_2/input/images/room3.jpg?raw=true)

## Output image:
![Output image] (https://github.com/najma510/DeepPixel/blob/master/deeppixel/image_stitching_2/output/room.jpg?raw=true)

## Approach

1. Reading multiple images ( in order)
2. Feature extraction
3. Matching correspondences between images
4. Compute Homography
5. Warping & Stitching

## Project Structure:

The `code` directory contains the main `pano.py` file. The `input` directory contains a `txtlists` directory which contains files having the paths to images in the panorama. These images are individually stored inside `images` directory.
The `output` directory stores the stitched images.


## Steps:

1. Clone this repository
```bash
git clone https://github.com/smaranjitghose/DeepPixel
```
2. Navigate to the project directory image_stitching_2
3. Install the required libraries in requirements.txt

Demo txtfile : file2.txt :
```
../../images/1.jpg
../../images/2.jpg
../../images/3.jpg
../../images/4.jpg
```
4. ### To Run:
```bash
python pano.py <filename.txt>
```
> for example
```bash
python pano.py <input/txtlists/file1.txt>
```
5. The stitched image (panorama) will be displayed.


## References:
[Multiple Image Stitching](https://kushalvyas.github.io/stitching.html)