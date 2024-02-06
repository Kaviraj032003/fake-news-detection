# Fake News Detection using Intel Patch, Scikit-learn, and Logistic Regression

## Overview

This project aims to create a fake news detection system using Intel optimized scikit-learn library and Logistic Regression. The detection model is built on a dataset containing both genuine and fake news articles, and it utilizes the power of Intel optimizations to enhance the performance of the logistic regression algorithm.

## Prerequisites

- Python 3.x
- Intel Distribution for Python
- Scikit-learn
- Pandas
- Numpy

## Installation

1. Install Python 3.x from [python.org](https://www.python.org/downloads/).
2. Install Intel Distribution for Python by following the instructions on the [Intel website](https://software.intel.com/content/www/us/en/develop/tools/distribution-for-python/choose-download.html).
3. Install required Python packages:

   ```bash
   pip install scikit-learn pandas numpy
   ```

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/fake-news-detection.git
   ```

2. Navigate to the project directory:

   ```bash
   cd fake-news-detection
   ```

3. Download and prepare the dataset (ensure it has columns for 'text' and 'label').

4. Run the following command to train the model:

   ```bash
   python train_model.py -d path/to/dataset.csv
   ```

   Replace `path/to/dataset.csv` with the actual path to your dataset.

5. After training, you can evaluate the model's performance:

   ```bash
   python evaluate_model.py -d path/to/test_dataset.csv -m path/to/saved_model.pkl
   ```

   Replace `path/to/test_dataset.csv` with the path to your test dataset, and `path/to/saved_model.pkl` with the path where the trained model is saved.

## Model Optimization with Intel Patch

1. Ensure you have the Intel Distribution for Python installed.

2. Apply Intel optimization patches to the scikit-learn library:

   ```bash
   conda install -c intel scikit-learn
   ```

3. Re-run the training and evaluation steps mentioned above to leverage Intel optimizations.

## Acknowledgments

- Thanks to Intel for providing optimized libraries that enhance the performance of machine learning algorithms.
