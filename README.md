# Emotional Detection AI

This repository contains an emotional detection AI system that analyzes facial expressions to identify emotions.

## Getting Started

### Prerequisites
- Python 3.8+
- Required packages (install via pip install -r requirements.txt)

### Dataset
The model is trained on the FER2013 dataset from Kaggle. To download the dataset:

1. Create a Kaggle account if you don't have one
2. Download the dataset from: [https://www.kaggle.com/datasets/msambare/fer2013](https://www.kaggle.com/datasets/msambare/fer2013)
3. Place the dataset in the data/ directory

### Training
To train the model yourself:

1. Open the training notebook (train_emotion_model.ipynb)
2. Follow the instructions in the notebook to train the model
3. The trained model will be saved as an .h5 file that can be used in the main application

### Model Files
The pre-trained model is stored in a .h5 file format. To use it:

1. Download or train the model (see Training section)
2. When using the model in your Python scripts, load it with:
   python
   from tensorflow.keras.models import load_model
   
   # Load the pre-trained model
   model = load_model('path/to/emotion_model.h5')

### Running the Application
Execute the main Python script to run the application:

bash
python main.py


## Project Structure
- data/ - Directory for the dataset
- models/ - Directory for saved model files (.h5)
- train_emotion_model.ipynb - Jupyter notebook for model training
- main.py - Main application script
- requirements.txt - List of dependencies
