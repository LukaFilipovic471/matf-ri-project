# Deep Dream with PyTorch

This repository contains a PyTorch implementation of the Deep Dream algorithm. Deep Dream is an image generation technique that enhances patterns in an image by optimizing the input image to maximize the activation of specific layers within a neural network.

## Requirements

- Python 3.x
- PyTorch
- torchvision
- Pillow (PIL)
- NumPy
- Matplotlib

Install the required dependencies using the following command:

```bash
pip install torch torchvision Pillow numpy matplotlib
```

## Usage

### 1. Clone the Repository
```bash
git clone https://github.com/LukaFilipovic471/matf-ri-project.git
```

### 2. Run Deep Dream
Modify the `input_image_path`, `layer_index`, `iterations`, `learning_rate`, `octave_scale`, and `output_image_path` in the deepdream.ipynb file to suit your preferences.
```bash
# Specify the parameters
input_image_path = 'path/to/your/image.jpg'
layer_index = 10
iterations = 100
learning_rate = 0.01
octave_scale = 1.4
output_image_path = "path/to/output.jpg"
```

### 3. Visualize Results
The input image and the generated Deep Dream output will be displayed using Matplotlib.

## Code Overview

### DeepDream Class
The `DeepDream` class defines a PyTorch module for the Deep Dream model. It takes a pre-trained neural network and a layer index as input and extracts features from the network up to the specified layer.

### deep_dream Function
The `deep_dream` function performs the Deep Dream algorithm on an input image using the specified model and layer. It iteratively optimizes the input image to enhance patterns that activate the chosen layer.

### Set the Device and Load Pre-trained Model
The script sets the device to GPU if available, loads a pre-trained model (inception_v3 in this example), and sets it to evaluation mode.

### Display Input and Output Images
Matplotlib is used to display the input image and the final Deep Dream output side by side.

## References
##### <a href="https://en.wikipedia.org/wiki/DeepDream"> Deep Dream on Wikipedia </a>
##### <a href=https://www.tensorflow.org/tutorials/generative/deepdream> Deep Dream using Tensorflow</a>
##### <a href=https://pytorch.org/docs/stable/index.html> PyTorch Documentation</a>
