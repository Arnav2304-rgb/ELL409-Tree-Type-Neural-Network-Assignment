# Tree-Type Neural Network

Experiments with Prof. Jayadeva's tree-type neural network on Cats-vs-Dogs and CIFAR-10. Each tree node is a small MLP that corrects selected errors made by its parent.

## Notebooks

- **`notebook1.ipynb`** — Main CNN-backed version. A jointly trained CNN supplies shallow, mid, and deep feature views to correction nodes. Includes overfitting, double-descent, occlusion-sensitivity, and model-size experiments.
- **`notebook2.ipynb`** — CPU-oriented handcrafted-feature version using colour-grid appearance, HOG, Sobel/Laplacian detail, LBP texture (Cats-vs-Dogs only), and a raw-pixel PCA reserve. CIFAR-10 uses ECOC to decode the 10 classes.

## Running

Run cells from top to bottom in Jupyter, Kaggle, or Colab. The first notebook benefits from a GPU; the second is designed for CPU use. Dataset, feature, and experiment caches are reused between runs when available; setup cells contain the relevant loading and dependency steps.
