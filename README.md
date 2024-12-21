![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)

# Next Word Predictor

## Overview
This project evaluated the performance of several recurrent neural network (RNN) architectures for next-word prediction. Specifically, we compared standard RNNs, stacked RNNs, Long Short-Term Memory (LSTM) networks, stacked LSTMs, Gated Recurrent Units (GRUs), and stacked GRUs. These models were trained on a 500-line corpus of narrative text to assess their ability to capture sequential dependencies in language. Results indicated that performance in predicting the subsequent five words was limited across all architectures, particularly given the small training dataset. This comparison underscores the challenge of training complex sequence models with limited data and highlights the need for evaluation metrics that go beyond simple next-word accuracy, emphasizing the importance of semantic analysis and contextual understanding for a more comprehensive model assessment.

## Features
- Processes text using TensorFlow and Keras for robust tokenization and modeling.
- Adapts to different datasets, allowing flexibility in application.
- Generates contextually accurate predictions for creative or analytical tasks.

## Dataset
The dataset used is a custom collection of lore narratives, featuring descriptions of characters and storylines. This provides a rich source of linguistic patterns for the model to learn from.

## How It Works
1. **Preprocessing**: Text is broken into tokens (individual words or characters) to form a structured input.
2. **Training the Model**: The core architecture uses a Recurrent Neural Network (RNN) with Long Short-Term Memory (LSTM) units. This helps the model understand relationships between words over time. The setup also includes embedding layers for word representation and dense layers for generating predictions.
3. **Making Predictions**: After training, the model predicts the next word based on a given input sequence, ensuring the output aligns with the input's context.

## Requirements
- Python 3.8 or newer
- TensorFlow 2.x
- Install dependencies with:
  ```bash
  pip install -r requirements.txt
## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/kaulvishesh/Next_wrd_pred.git
## Results
The model predicts the next word for any input text. For instance, feeding it part of a sentence from the lore dataset will generate the next logical word based on its training.

## Contributing
Contributions are welcome! Fork the repository, create a branch, and submit a pull request to suggest improvements or add features.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgments
- TensorFlow and Keras for their powerful tools.
- The broader NLP community for inspiring advancements in language modeling.
