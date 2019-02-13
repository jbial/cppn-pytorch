# Compositional Pattern Producing Networks in Tensorflow
Generate high resolution, intensely stimulating images with random neural networks.

## Arguments
`python generate.py` takes as arguments:
* `--im-size`: Size of the image.
* `--batch-size`: Number of images to generate.
* `--n-dim`: Number of units per layer.
* `--z-dim`: Size of input latent vector.
* `--layers`: Number of layers in the network.
* `--channels`: Number of channels in output images.
* `--scale`: Scaling factor for the images.
* `--name`: Name of image for saving. Default is None, specify for saving.
* `--frames`: Number of frames for the gif. Default is None, specify an integer to save a gif file.

## Usage
Generating Images: `python generate.py` 

![alt text](https://github.com/jbial/cppn-pytorch/blob/master/images/tanhtanh_2.png)

Generating Gifs: `python generate.py --frames=10 --name="foo.gif"`

![alt text](https://github.com/jbial/cppn-pytorch/blob/master/gifs/tanhtanh.gif)


## Experiments
* I found the `--scale` and `--z-dim` parameter to have the most impact of visual effects.
* In general, the scale acts as a "zooming" parameter in the image space, and the z dimension acts a frequency parameter of generated image features

<p float="left">
  <img src="https://github.com/jbial/cppn-pytorch/blob/master/images/scale_1.jpg" width="128" />
  <img src="https://github.com/jbial/cppn-pytorch/blob/master/images/scale_2.jpg" width="128" /> 
  <img src="https://github.com/jbial/cppn-pytorch/blob/master/images/scale_3.jpg" width="128" />
  <img src="https://github.com/jbial/cppn-pytorch/blob/master/images/scale_4.jpg" width="128" />
</p>

## Acknowledgement

This project was adapted from [David Ha's amazing blog post](http://blog.otoro.net/2016/03/25/generating-abstract-patterns-with-tensorflow/)

