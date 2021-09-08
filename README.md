# CPPN

Playing around with generative art through
[compositional pattern-producing networks](https://blog.otoro.net/2016/03/25/generating-abstract-patterns-with-tensorflow/),
neural networks that map (x, y) -> (r, g, b).

Initially written in January 2021 to make desktop backgrounds.
Includes code and demos of symmetric CPPNs, using bitmaps as inputs, and animations, including looping.

## Files

 - `cppn_random.ipynb`: Random fully-connected networks, including enforcing symmetries.
 - `cppn_conv.ipynb`: Random convolutional networks.
 - `cppn_paramcircle.ipynb`: Using a controllable input channel to add structured patterns to the CPPN output.
 - `cppn_image.ipynb`: Using an image bitmap as the input coordinate, effectively using the CPPN as a nonlinear colormap for
   an existing raster.
 - `cppn_time.ipynb`: Making animations by running a CPPN with a time dimension. Animations can be looped by
   [walking parameters around a high-dimensional circle](https://www.youtube.com/watch?v=aP7n5ly_fiQ).
 - `cppn_styletransfer.ipynb`: Optimizing a CPPN to match the style of a target image. This one doesn't really work.
