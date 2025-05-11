# torch-anatomy
---
**Layer-by-layer visualizer for PyTorch models — Understand what each layer actually does.**

![torch-anatomy demo](assets/package-image.png)

[![PyPI](https://img.shields.io/pypi/v/torch-anatomy)](https://pypi.org/project/torch-anatomy/)
[![License](https://img.shields.io/github/license/harsk03/torch-anatomy)](LICENSE)

---

## 🚀 What is torch-anatomy?

**torch-anatomy** is an open-source Python tool to visualize the internal activations of any PyTorch CNN model, layer by layer.  
Perfect for ML students, researchers, and anyone curious about what their neural network is “seeing”!

---

## 📦 Install

```bash
pip install torch-anatomy
```

---

## 🧑‍💻 Quick Usage

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

---
## 🖼️ Examples Screenshots
![torch-anatomy demo](assets/layer_visualizations.png)
---

## 🔗 Links

- [PyPI Package](https://pypi.org/project/torch-anatomy/)
- [Main Code Repository](https://github.com/harsk03/torch-anatomy) (private repo for now !)
- [Jupyter Notebook Example](examples/demo.ipynb)

---

## 🙌 Contribute & Feedback

- Issues, suggestions, and PRs welcome!
- Contact: harshalkale2402@gmail.com or open an issue

---

## 📝 License

MIT
