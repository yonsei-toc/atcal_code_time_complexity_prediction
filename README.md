# @CAL: Advanced Code Time Complexity Prediction Approach Using Contrastive Learning (In Engineering Applications of Artificial Intelligence, Vol. 151, 110631, July 2025)

## Project Description
This repository contains the source code and dataset for implementing **@CAL**, a contrastive learning-based approach for code time complexity prediction.  
@CAL introduces a novel training methodology for the code time complexity prediction task. This task involves predicting the worst-case time complexity of given source code as a multi-class classification problem.

## Dataset
The repository provides a benchmark dataset comprising Python and Java source code for time complexity prediction tasks. The dataset is designed to classify input source code into one of the following time complexity categories:
- O(1)
- O(n)
- O(n²)
- O(n³)
- O(log n)
- O(n log n)
- O(2ⁿ)

The preprocessed dataset can be found in the `preprocessed_data/` directory.

## Experiment Setup
Before running an experiment, navigate to the corresponding folder for the specific experimental setup. 
For example, if you want to perform the cross-dataset experiment, move to the `cross_dataset/` directory.

## Project Structure
```
.
├── train.py                   # Main execution file
├── train_config.py            # Hyperparameter and experiment configuration settings
├── collate_fns_complexon.py   # Collate functions for source code input padding
├── dataset_complexcon.py      # Dataloader implementation
├── model.py                   # Pre-trained language model encoder definition
├── loss_complexcon.py         # Contrastive learning-based @CAL loss implementation
├── util.py                    # Utility functions
├── requirements.txt           # Required libraries and dependencies
└── preprocessed_data/         # Directory containing the preprocessed dataset
```

## Features
- Implementation of contrastive learning-based approach for time complexity prediction
- Support for both Python and Java source code analysis
- Multi-class classification for seven different time complexity categories
- Preprocessed benchmark dataset for training and evaluation

## Requirements
To set up the environment, install the required libraries using:
```bash
pip install -r requirements.txt
```

# Hyperparameter Configuration
To adjust the hyperparameters and experiment settings, modify the 
```bash
train_config.py
```
file accrodingly.

## Usage
Run train.py
```bash
python train.py
```

## 🖊 Citation
```text
@article{park2025complexity,
    title = {Advanced code time complexity prediction approach using contrastive learning},
    author = {Shinwoo Park and Joonghyuk Hahn and Elizabeth Orwig and Sang-Ki Ko and Yo-Sub Han},
    journal = {Engineering Applications of Artificial Intelligence},
    year = {2025},
    volume = {151},
    pages = {110631},
    issn = {0952-1976},
    doi = {https://doi.org/10.1016/j.engappai.2025.110631},
    url = {https://www.sciencedirect.com/science/article/pii/S0952197625006311},
}
```
