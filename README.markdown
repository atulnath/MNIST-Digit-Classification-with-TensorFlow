# MNIST Digit Classification with TensorFlow

This project implements a neural network using TensorFlow to classify handwritten digits from the MNIST dataset.

## Overview

The code builds a simple feedforward neural network to recognize handwritten digits (0-9) from the MNIST dataset. It includes data preprocessing, model training, evaluation, and visualization of results.

## Requirements

- Python 3.x
- TensorFlow
- NumPy
- Matplotlib

Install dependencies using:
```bash
pip install tensorflow numpy matplotlib
```

## Usage

1. Clone the repository:
```bash
git clone https://github.com/your-username/mnist-digit-classification.git
cd mnist-digit-classification
```

2. Run the script:
```bash
python mnist_classification.py
```

## Code Structure

The main script (`mnist_classification.py`) performs the following steps:

1. **Data Loading**: Loads the MNIST dataset using `keras.datasets.mnist.load_data()`.
2. **Data Preprocessing**: Normalizes pixel values to the range [0, 1].
3. **Model Definition**: Creates a Sequential model with:
   - Input layer: 28x28 images
   - Flatten layer: Converts 2D images to 1D (784 neurons)
   - Dense layer: 128 neurons with ReLU activation
   - Output layer: 10 neurons with softmax activation
4. **Model Compilation**: Uses Adam optimizer and sparse categorical crossentropy loss.
5. **Training**: Trains the model for 10 epochs with a batch size of 64 and 20% validation split.
6. **Evaluation**: Evaluates the model on the test set.
7. **Prediction**: Generates predictions and visualizes sample test images.
8. **Visualization**: Plots training/validation loss and accuracy curves.

## Results

- The model achieves high accuracy on the test set (typically ~97-98% after 10 epochs).
- Loss and accuracy plots are generated to visualize training progress.

## Example Visualizations

- Sample digit images from the dataset are displayed using `matplotlib`.
- Training and validation loss/accuracy are plotted to assess model performance.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The MNIST dataset is provided by TensorFlow/Keras.
- Built with TensorFlow and inspired by standard deep learning tutorials.