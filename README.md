# keras2tikz
Generate (hopefully) readable tikz code for DNN layer diagrams.

Adapted to run on Tensorflow 2.1.
Python 3.6.

## Why?

Keras has a `summary` and a [builtin graphviz export](https://github.com/fchollet/keras/blob/master/keras/utils/vis_utils.py). Both show the input and output shapes of all layers. However, many papers show the layer parameters, so I've added some common parameters like hidden units (Dense + Recurrent), Kernel size and number of filter (Convolutional), Pooling Dimensions... to the output graph...

## Usage

```shell
python vgg16_model.h5
```

```shell
python resnet18_model.h5
```

The output .tex file in tex_output can be compiled with pdfLaTeX.

![vgg16](https://cloud.githubusercontent.com/assets/72940/26532609/61ff71aa-4405-11e7-9827-6cc4b12550dc.png)
