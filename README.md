# Advisor Chatbot Project

### A Natural Language Processing-Based Solution for Academic Advising

## Project Overview

This project is an AI-powered chatbot designed to assist students with academic advising. The chatbot leverages Natural Language Processing (NLP) techniques and a Long Short-Term Memory (LSTM) Recurrent Neural Network (RNN) model to provide accurate and contextual responses to common advising questions.

### Key Features
- **24/7 Availability:** The chatbot is available round the clock to answer questions related to course registration, campus events, academic policies, and more.
- **Custom FAQ Dataset:** The model has been trained on a custom dataset tailored specifically for academic advising, alongside standard NLP datasets.
- **User-Friendly Interaction:** The chatbot is designed to understand natural language input and provide precise answers, enhancing the overall advising experience.

## Technologies Used

- **Python**: Core programming language for the project.
- **TensorFlow/Keras**: Used for building and training the LSTM model.
- **NLTK (Natural Language Toolkit)**: Employed for text preprocessing, including tokenization, stopword removal, and lemmatization.
- **scikit-learn**: Used for vectorization and similarity measurements.
- **Git/GitHub**: Version control and project collaboration.

## Project Structure

The project is structured as follows:

├── Data/ # Datasets and logs

├── Models/ # Saved model versions

├── Preprocessing.py # Script for data preprocessing

├── NLP.py # Script for NLP-related functions

├── ML.py # Script for machine learning model functions

├── Train.py # Script for training the chatbot

├── Chatbot.py # Main script to run the chatbot

├── README.md # Project documentation


## Setup Instructions

### 1. Clone the Repository

Start by cloning this repository to your local machine:

```bash
git clone https://github.com/nat2k1/Advisor-Chatbot.git
cd Advisor-Chatbot
```
### 2. Install Required Dependencies

Make sure you have Python installed. Then, install the required libraries:
```bash
pip install -r requirements.txt
```

### 3. Running the Chatbot

To launch the chatbot, simply run:
```bash
python Chatbot.py
```

### 4. Training the Model (Optional)

If you want to train the model from scratch, use the following command:
```bash
python Train.py
```

This will preprocess the data, train the model, and save the best-performing version.
### 5. Updating the Model

To update the model with new data or configurations, ensure the latest dataset is in the Data/ folder, then run the training script again.

## Model Performance

The model has been trained on a combination of the IMDB dataset and a custom FAQ dataset. It achieves the following metrics:

    Validation Accuracy: ~87%
    Validation Loss: ~0.59
    Training Time: Approximately 30 minutes per epoch on average hardware

## Challenges and Solutions

### Low Initial Accuracy
Our initial attempts resulted in low accuracy (~50%). We addressed this by switching from a SimpleRNN to an LSTM architecture, which significantly improved performance.

### Dataset Limitations
We encountered challenges with the availability of relevant datasets for academic advising. To overcome this, we merged various sources and created a custom FAQ dataset.

### Training Time
LSTM models can be computationally intensive. We optimized our training by adjusting batch sizes, epochs, and leveraging hardware acceleration.

## Contributing

Contributions are welcome! Please fork this repository, create a new branch, and submit a pull request with your improvements.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact Information

For further questions or collaborations, please reach out via GitHub: nat2k1.
