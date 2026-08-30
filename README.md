# Image Classification with PyTorch

This notebook trains a small convolutional neural network on the CIFAR-10
dataset and uses it to classify the included sample images.

## Run the notebook

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\\Scripts\\activate
pip install -r requirements.txt
jupyter notebook Main.ipynb
```

Run the cells from top to bottom. CIFAR-10 is downloaded into `./data` on the
first run, and training writes `trained_net.pth`. The evaluation loader keeps a
stable order, and custom images are converted to RGB before inference so
grayscale and RGBA inputs work with the three-channel model.
