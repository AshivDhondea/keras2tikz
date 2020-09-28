# keras2tikz
Generate (hopefully) readable tikz code for DNN layer diagrams.

Adapted to run on Tensorflow 2.

I (Ashiv Hans) used Python 3.6 and Tensorflow 2.1.

## Why?

Keras has a `summary` and a [builtin graphviz export](https://github.com/fchollet/keras/blob/master/keras/utils/vis_utils.py). Both show the input and output shapes of all layers. However, many papers show the layer parameters, so I've added some common parameters like hidden units (Dense + Recurrent), Kernel size and number of filter (Convolutional), Pooling Dimensions... to the output graph...

## Usage

For a VGG16:
```shell
python vgg16_model.h5
```
For a ResNet18:
```shell
python resnet18_model.h5
```

The output .tex file in tex_output can be compiled with pdfLaTeX.

ResNet18 on the left and VGG16 on the right.
![resnet18](https://github.com/AshivDhondea/keras2tikz/blob/master/png_display/resnet18_model._tikz-1.png)
![vgg16](https://github.com/AshivDhondea/keras2tikz/blob/master/png_display/vgg16_model._tikz-1.png)
