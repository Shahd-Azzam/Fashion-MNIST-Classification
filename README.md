# Fashion-MNIST Classification Using Neural Networks

## Project Overview
This project explores image classification using a neural network trained on the Fashion-MNIST dataset. The goal is to study how different model configurations and training settings affect classification performance.

## Dataset
Fashion-MNIST contains grayscale images of clothing items belonging to 10 classes. Each image has a resolution of 28 × 28 pixels.

## Experiments
The project includes 10 tasks exploring different neural network configurations and training strategies, including:

- Baseline model
- Number of training epochs
- Early stopping
- Number of hidden neurons
- Batch size
- Optimizer selection
- Activation functions

## Model Evaluation
The selected configuration was **Hidden neurons = 128**.

| Metric | Result |
|---|---:|
| Test Accuracy | 87.12% |
| Test Loss | 0.3703 |

These results correspond to the final test evaluation recorded during the experiment.

## MLflow Experiment Tracking
MLflow was used to track and compare the existing experiments, including model parameters, validation metrics, training duration, and training history when available.

To open the local MLflow UI, start the MLflow server from the project directory:

```bash
python -m mlflow server --backend-store-uri sqlite:///mlflow.db --host 127.0.0.1 --port 5000
```

Then open:

http://127.0.0.1:5000

The local MLflow database and run artifacts are not included in this repository by default.

## Installation

Install the required packages:

```bash
pip install -r requirements.txt
```

## How to Run
1. Clone or download this repository.
2. Install the required packages.
3. Open the Jupyter Notebook in VS Code.
4. Run the notebook cells in order to reproduce the experiments.

**Note:** Reproducing the experiments requires running the training cells. The previously recorded MLflow runs are stored locally and are not automatically available to other users.

## Technologies
- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- MLflow
- Jupyter Notebook

## Privacy
No local MLflow database, virtual environment, credentials, or machine-specific configuration files should be committed to this repository.
