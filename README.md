## FashionMNIST Classification with Neural Networks (PyTorch)

This project focuses on image classification on the FashionMNIST dataset using neural networks implemented in PyTorch. The comparison is between the performance of a Multi-Layer Perceptron (MLP) with a Convolutional Neural Network (CNN). This project demonstrates the superior effectiveness of convolutional architectures for image-based learning tasks.

Several techniques are employed to improve training stability and generalization, including L2 regularization, dropout, and batch normalization. The ReLU activation function is used throughout the networks to mitigate the vanishing gradient problem and enable efficient training of deep architectures.

Hyperparameter tuning is carried out using 3-fold cross-validation combined with Optuna, allowing for an automated and systematic search for optimal model configurations.

Beyond performance evaluation, the project includes an analysis of the learned representations. We visualize convolutional filters, feature maps, and the resulting latent feature space using dimensionality-reduction techniques to gain insight into how the networks encode and separate different classes.

## Dataset

This project uses the **FashionMNIST** dataset, a widely adopted benchmark for image classification tasks. The dataset consists of **28×28 grayscale images** belonging to **10 different clothing categories**.

The dataset is split into **60,000 training samples** and **10,000 test samples**. Images are normalized and loaded automatically using the `torchvision.datasets.FashionMNIST` interface.

## Key Features

- **FashionMNIST classification** using neural networks implemented in **PyTorch**
- **Comparison between MLP and CNN architectures**, highlighting the advantages of convolutional models for image data
- **Regularization techniques** including L2 weight decay and dropout to reduce overfitting
- **ReLU activation function** to prevent vanishing gradients and enable efficient deep learning
- **Batch normalization** applied before activation layers to improve training stability
- **Hyperparameter optimization** using 3-fold cross-validation combined with **Optuna**
- **Model interpretability analysis**, including visualization of convolutional kernels and feature maps
- **Feature space exploration** using dimensionality-reduction techniques to study class separation and clustering
