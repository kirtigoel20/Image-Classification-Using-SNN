# Spike-Based Image Classification Using Spiking Neural Networks


## 📌 Project Overview

This project explores image classification using Spiking Neural Networks (SNNs), inspired by the information-processing mechanisms of biological neurons.

The project investigates different spiking neuron models and learning strategies using PyTorch and snnTorch. It is designed to compare Leaky Integrate-and-Fire (LIF) and Adaptive Leaky Integrate-and-Fire (ALIF) neurons, along with surrogate-gradient learning and Reward-Modulated Spike-Timing-Dependent Plasticity (R-STDP).

The experiments focus on the MNIST and CIFAR-10 image datasets.

## 🎯 Objectives

- Implement SNN architectures for image classification.
- Compare LIF and ALIF neuron models.
- Explore surrogate-gradient learning and R-STDP.
- Investigate Poisson rate coding and direct input encoding.
- Visualize spike activity and membrane potential dynamics.
- Analyze model accuracy, training behavior, and computational time.

## 🛠️ Technologies Used

- Python
- PyTorch
- snnTorch
- Torchvision
- NumPy
- Matplotlib
- Hugging Face Datasets
- Google Colab

## 🧠 Model Architecture

The SNN architecture consists of:

| Layer | Description | Neurons |
|---|---|---:|
| Input | Encoded image input | 784 for MNIST; 2304-dimensional features for CIFAR-10 |
| Hidden | Fully connected spiking layer | 256 |
| Output | Fully connected spiking layer | 10 |

The SNN contains 266 spiking neurons per model, excluding the input representation.

For CIFAR-10, a convolutional neural network (CNN) backbone extracts image features before they are passed to the SNN.

## 🔬 Experimental Design

The notebook explores combinations of the following components.

### 1. Spiking Neuron Models

- **LIF (Leaky Integrate-and-Fire):** Models membrane potential dynamics and spike generation.
- **ALIF (Adaptive Leaky Integrate-and-Fire):** Incorporates an adaptive firing threshold.

### 2. Learning Strategies

- **Surrogate Gradient:** Uses a differentiable approximation of the spike function to enable gradient-based learning.
- **R-STDP:** Explores reward-modulated spike-timing-dependent weight updates.

### 3. Spike Encoding

- **Poisson Rate Coding:** Represents input intensities through stochastic spike generation.
- **Direct Encoding:** Repeats continuous input values across simulation timesteps.

### 4. Datasets

- **MNIST:** Handwritten digit classification.
- **CIFAR-10:** Classification of images across ten object categories.

The notebook defines eight planned experiment configurations covering the two datasets, two neuron models, and two learning strategies. The successful execution and evaluation of each configuration must be verified before drawing comparative conclusions.

## 📊 Visualizations and Analysis

The notebook includes visualizations for:

- SNN architecture and neuron counts.
- LIF versus ALIF membrane potential dynamics.
- Spike encoding strategies.
- Training accuracy and loss.
- Final test accuracy comparisons.
- Training time and efficiency analysis.
- Confusion matrix analysis.

Quantitative results and comparisons should be added after the corresponding experiments have executed successfully.

## 🚀 How to Run the Project

The notebook is designed to run in Google Colab.

1. Open `SNN_Image_Classification.ipynb` in Google Colab.
2. Enable a GPU runtime if available.
3. Install the required packages:

   ```python
   !pip install snntorch datasets
   ```

4. Run the notebook cells in sequence.
5. Verify that the dataset loaders initialize successfully.
6. Execute the training and evaluation experiments.
7. Review the generated visualizations and measured results.

**Note:** Dataset access, package versions, GPU availability, and notebook execution state may affect reproducibility.

## 📁 Repository Structure

```text
SNN-Image-Classification/
├── README.md
└── SNN_Image_Classification.ipynb
```

## 🔮 Future Improvements

- Complete and validate all planned experiments.
- Improve dataset-loading reliability.
- Compare neuron models and learning strategies using consistent evaluation settings.
- Add verified test accuracy, training time, and confusion matrices.
- Explore larger SNN architectures and additional encoding strategies.

## 👩‍💻 Author

**Kirti Goel**

B.Tech in Computer Science and Engineering  
Jaypee University of Information Technology (JUIT)
