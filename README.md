# Paintify
This Python project recreates an image in the style of a brush painting. It achieves this by sampling points from the original image and placing coloured brush strokes on a blank canvas. It has two implementations. One uses the PIL Image library while the other utilizes Numpy arrays. Both follow the same ideas.

## How It Works
The code samples points across the image at set intervals. A big interval means fewer sample points, so the painting looks rougher and more artistic. A small interval means more sample points, so the result keeps more detail and looks closer to the original image. At each point it reads the colour of the pixel. It then takes a brush stroke image, recolours it to match the pixel it is copying and places it on a blank canvas. This is repeated to a build a painted version of the image.

The PIL version handles strokes with simple image operations like resizing, recolouring, rotating, and pasting. It is easy to follow and good for learning. The Numpy version converts all images to arrays and uses array slicing and custom mixing of colours to blend brush strokes at the pixel level. It is faster and gives more control. Both versions follow the same process and support options like random sample order, random brush rotation, borders, watermarks, batch, processing, and saving or showing the final result.


## Features
- Two full implementations
- Random sample order
- Random brush rotation
- Optional border
- Image comparison
- Added watermark
- Progress tracking
- Bulk processing

## Examples
![Flower](Images/Image/image_1_new_2.jpg)

![Train](Images/Image/image_2_new_2.jpg)

![Trees](Images/Image/image_3_new_2.jpg)



