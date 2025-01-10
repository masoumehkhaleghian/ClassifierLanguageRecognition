# ClassifierLanguageRecognition

## Overview
This repository contains a TensorFlow-based machine learning model for detecting the language of a given text. The model has been trained on data to classify text into the following languages:

- Estonian
- Swedish
- Thai
- Tamil
- Dutch
- Japanese
- Turkish
- Latin
- Urdu
- Indonesian
- Portuguese
- French
- Chinese
- Korean
- Hindi
- Spanish
- Pashto
- Persian
- Romanian
- Russian
- English
- Arabic
- Italian

The training dataset is located in the Dataset folder.

## Features
- Detects 23 different languages from textual data.
- Built and trained using TensorFlow.
- Dataset and model architecture are included for reproducibility.

## Project Structure
```
ClassifierLanguageRecognition/
|-- Dataset/               # Folder containing the training data
|   |-- data.csv           # Main dataset used for training the model
|-- Model/                 # Folder for saving the trained model 
|-- ClassifierLanguageRecognition.ipynb # Main script to train and test the model
|-- requirements.txt       # Python dependencies
|-- README.md              # Project documentation
```

## Getting Started

### Prerequisites
- Python 3.8.20
- TensorFlow 2.x
- Pandas
- NumPy
- Scikit-learn

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/masoumehkhaleghian/ClassifierLanguageRecognition.git
   cd ClassifierLanguageRecognition
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Usage

1. Prepare the dataset:
   - Ensure the Dataset/data.csv file is present and formatted correctly with two columns: `sentence` (text data) and `language` (language labels).

2. Train the model:
   - Open the `ClassifierLanguageRecognition.ipynb` notebook and run all cells to train the model.

3. Test the model:
   - Modify the notebook to include your test cases or integrate the trained model into your application.

### Example Input
```csv
sentence,language
"Hello, how are you?",english
"Bonjour, comment ça va?",french
"السلام عليكم",arabic
```

### Example Output
For the input "Bonjour, comment ça va?", the output will be:
```
Predicted Language: French
```

## Model Details
- Framework: TensorFlow
- Algorithm: Neural network classifier
- Evaluation Metrics: Accuracy, F1-score

