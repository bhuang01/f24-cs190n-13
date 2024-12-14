# Environment
- Python 3.10.15

# Reproduction Instructions

## Download Data and Setup

1. Clone and download the dataset from the [USTC-TFC2016 repository](https://github.com/yungshenglu/USTC-TFC2016)

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Data Preparation

3. Build dataframe by concatenating datasets.
    - Load individual datasets into a single DataFrame, ensuring correct label assignment for each traffic category. 
    - Combine the DataFrames into one main dataframe that contains all of network traffic data.

4. Feature Selection and Preprocessing
   - Select relevant features for training
   - Preprocess the data:
        - aggregate information on packets into flows and use them as a datapoint in the training and test sets.

## Model Pipeline

5. Set up pipeline
   - Split data (train/validation/test)
   - Feature scaling 

6. Model Training
    - Execute the training process with training dataset

7. Model Analysis
   - Evaluate model performance and analyze which features affected model most significantly.