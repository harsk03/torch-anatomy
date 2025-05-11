# torch-anatomy

# torch-anatomy

**Layer-by-layer visualizer for PyTorch models — Understand what each layer actually does.**

![PyPI](https://img.shields.io/pypi/v/torch-anatomy)
![License](https://img.shields.io/github/license/harsk03/torch-anatomy)

## Install

```bash
pip install torch-anatomy
```

## Usage

```python
from torch_anatomy import visualize_layers
from torchvision import models

model = models.resnet18(pretrained=True)
visualize_layers(
    model=model,
    input_image='dog.jpg',
    layers_to_show=['Conv2d', 'ReLU'],
    channels_per_layer=6,
    colormap='inferno',
    show_colorbar=True
)
```

Or from CLI:

```bash
torch-anatomy --model resnet18 --image dog.jpg
```

## Features
- Plug-and-play for any PyTorch CNN
- Visualizes feature maps for key layers
- Customizable channels, colormap, and more

## License
MIT
