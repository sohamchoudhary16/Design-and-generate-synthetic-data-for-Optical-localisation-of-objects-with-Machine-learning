# Design-and-generate-synthetic-data-for-Optical-localisation-of-objects-with-Machine-learning

To automatically generate data (pictures and annotation files) for shiny objects (Shafts) with high quality and significant quantity fluctuations within a predetermined time range.

## Requirements
Blender 2.8 or later (https://www.blender.org/download/)

## Implementation
* Importing required libraries
Baking of dynamics
Randomly hiding the shafts so that images with different number of shafts will be produced
Randomizing the orientation so that the dynamics will be changed
Creating compositor nodes which filters the object to get only edges
finding out pixel coordinates, angle w.r.to x-axis and also xy plane and confidence intervals
writing all the data into a textfile
rendering a greyscale image(256x256)
finally unhiding the shafts to make them ready for the next iteration
