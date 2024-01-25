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

