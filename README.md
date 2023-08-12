# Simple AI (Shakespearean) Text Generator
This Python script demonstrates a simple text generation model using an LSTM neural network to generate poetic text. The model is trained on a Shakespearean text dataset. Given an initial seed sequence, the model predicts the next characters based on the input and generates poetic text. The script will load the pre-trained model and generate poetic text with varying levels of creativity (controlled by the temperature parameter). The generated text will be displayed for different temperature values.

# Libraries Used #
- NumPy
- TensorFlow 2.x
- Random

# Code Overview #
The code is divided into the following sections:

**Data Preparation:** Download the Shakespearean text dataset, preprocess it, and create the necessary dictionaries for character encoding.

**Model Architecture:** Build a simple LSTM-based model using Keras. Compile the model with categorical cross-entropy loss and RMSprop optimizer.

**Model Training:** Train the model on the prepared data using the compiled architecture. Save the trained model to a file.

**Text Generation:** Load the trained model and implement a function to generate poetic text. The function samples characters based on predicted probabilities.

**Generate Text:** Generate poetic text for different temperature values to control the level of creativity in the generated text.

# Adjusting Parameters #
- **'SEQ_LENGTH':** The length of the input sequence.
- **'STEP_SIZE':** The step size for creating training sequences.
- **'temperature':** A parameter controlling the creativity of generated text. Lower values (e.g., 0.2) produce more "experimental" text, while higher values (e.g., 1.0) produce more "safe" text.

# Results #
The script will display generated poetic text for different temperature values, allowing you to observe the impact of temperature on the creativity and randomness of the generated text.
