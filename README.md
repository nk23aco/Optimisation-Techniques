# Optimisation-Techniques
Optimization Techniques and role of hyperparamter

# Optimizer Comparison in Deep Learning

This project explores and compares the performance of different optimization techniques (Adam, SGD, RMSprop, Batch Gradient Descent, Mini-Batch Gradient Descent) for training a neural network on the California Housing dataset. The goal is to identify the best optimizer based on the Mean Squared Error (MSE) and analyze their behavior.

## Table of Contents
- [Overview](#overview)
- [Optimizers Tested](#optimizers-tested)
- [Results](#results)
- [Loss Curves](#loss-curves)
- [How to Run the Code](#how-to-run-the-code)
- [Dependencies](#dependencies)

## Overview
The California Housing dataset is a regression problem where the target variable represents the median house value in various districts. The neural network is built using TensorFlow and trained with various optimizers to compare their performance. Loss vs. epochs plots are generated for each optimizer to analyze convergence behavior.

## Optimizers Tested
The following optimization techniques were tested:
1. **Adam**
2. **Stochastic Gradient Descent (SGD)**
3. **RMSprop**
4. **Batch Gradient Descent**
5. **Mini-Batch Gradient Descent**

## Results
| **Optimizer**            | **MSE**              |
|---------------------------|----------------------|
| **Adam**                 | **0.2925**           |
| SGD                      | 0.3384               |
| RMSprop                  | 0.3005               |
| Batch Gradient Descent   | 0.4932               |
| Mini-Batch Gradient Descent | 0.3017            |

### Key Findings
- **Adam** achieved the lowest MSE, making it the best optimizer for this task.
- **Batch Gradient Descent** performed the worst due to its slow convergence and sensitivity to learning rate.
- **SGD** and **Mini-Batch Gradient Descent** provided reasonable results but required careful tuning.
- **RMSprop** performed well, closely following Adam in terms of MSE.

## Loss Curves
Loss vs. epochs plots were generated for each optimizer to visualize their convergence behavior. Adam and RMSprop showed the fastest convergence, while Batch Gradient Descent was significantly slower.

## How to Run the Code
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/optimizer-comparison.git
   ```
2. Navigate to the project directory:
   ```bash
   cd optimizer-comparison
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the main script:
   ```bash
   python main.py
   ```
5. View the results and generated plots.

## Dependencies
- Python 3.8+
- TensorFlow
- Keras Tuner
- Scikit-learn
- Matplotlib
- NumPy

## Acknowledgments
- **California Housing Dataset**: Provided by Scikit-learn.
- **Keras Tuner**: For hyperparameter tuning.

## License
This project is licensed under the MIT License.
