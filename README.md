# Brush Paintify
This project recreates an image in the style of a brush painting. It achieves this by sampling points from the original image and placing coloured brush strokes on a blank canvas. It has two implementations. Both are in Python and follow the same ideas. One uses the PIL Image library while the other utilizes Numpy arrays.

## How It Works
The code samples points across the image at set intervals. A big interval means fewer sample points, so the painting looks rougher and more artistic. A small interval means more sample points, so the result keeps more detail and looks closer to the original image. At each point it reads the colour of the pixel. It then takes a brush stroke image, recolours it to match the pixel it is copying and pastes it on a blank canvas. This is repeated as many times as needed to a build a painted version of the original image.

The PIL version handles strokes with simple image operations like resizing, recolouring, rotating, and pasting. It is easy to follow and good for learning. The Numpy version converts all images to arrays and uses array slicing and custom mixing of colours to blend brush strokes at the pixel level. It is faster and gives more control. Both versions follow the above process and support the same options.

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
![Puppies](Images/Image/puppies.jpg)

![Flower](Images/Image/image_1_new_2.jpg)

![Train](Images/Image/image_2_new_2.jpg)

![Trees](Images/Image/image_3_new_2.jpg)

![Coast](Images/Image/image_7_new_2.jpg)
