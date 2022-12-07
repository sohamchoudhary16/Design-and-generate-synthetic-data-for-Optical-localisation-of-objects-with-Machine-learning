# Design-and-generate-synthetic-data-for-Optical-localisation-of-objects-with-Machine-learning

To automatically generate data (pictures and annotation files) for shiny objects (Shafts) with high quality and significant quantity fluctuations within a predetermined time range.

## Requirements
Blender 2.8 or later (https://www.blender.org/download/)

## Implementation
* The required libraries are imported
* Dynamics are baked according to need
* Shafts are hidden randomly in every run such that varying number or quantities of shafts are produced
* The orientation is randomised such that the dynamics will be varied
* Compositor nodes are created that filter the objects to read on the edged
* Pixel coordinates, angle of orientation of shafts with respect to x-axis and xy plane and confidence intervals/thresholds after the shafts have aligned themselves in the bucket are found
* All the data is written in a text file
* Greyscale images of size 256x256 are rendered
* The shafts are set to unhide for the next iteration

## Dimensions of parameters in the text file 
* class
* x,y pixel coordinates
* angle of shaft with respect to x-axis
* angle of shaft with respect to xy plane
* confidence interval- 1(number of visible vertices to maximum number of visible vertices on the longer edges of shaft)
* confidence interval- 2(number of visible vertices to maximum number of visible vertices on the smaller edges of shaft)
