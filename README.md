# AI Chatbot for Resume Questions

This repository contains the code for an AI Chatbot designed to answer questions about a resume. It utilizes natural language processing (NLP) techniques and a neural network model to understand user queries and provide relevant responses based on predefined intents and patterns.

## Files

* **`chatbot.py`**: This file contains the code for running the trained chatbot. It loads the model, words, classes, and intents, and then interacts with the user.
* **`train.py`**: This file contains the code for training the chatbot model. It processes the intents, builds the vocabulary, trains a neural network, and saves the model.
* **`intents.json`**: This file stores the intents, patterns, and responses used by the chatbot.
* **`words.pkl`**: This file stores the list of words used in the chatbot's vocabulary (serialized using pickle).
* **`classes.pkl`**: This file stores the list of intent classes (serialized using pickle).
* **`chatbot_model.h5`**: This file stores the trained neural network model.
* **`.gitignore`**: This file tells git what files to ignore, such as the virtual enviroment.

## Setup and Installation

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/Ra-Verse/AI-chatbot.git](https://github.com/Ra-Verse/AI-chatbot.git)
    cd AI-chatbot
    ```

2.  **Create a virtual environment (recommended):**

    ```bash
    python -m venv .venv
    ```

3.  **Activate the virtual environment:**

    * **On Windows:**

        ```bash
        .venv\Scripts\activate
        ```

    * **On macOS and Linux:**

        ```bash
        source .venv/bin/activate
        ```

4.  **Install the required dependencies:**

    ```bash
    pip install tensorflow nltk numpy scikit-learn
    nltk.download('punkt')
    nltk.download('wordnet')
    ```

5.  **Train the model (if needed):**

    ```bash
    python train.py
    ```

6.  **Run the chatbot:**

    ```bash
    python chatbot.py
    ```

## Usage

Once the chatbot is running, you can type questions related to the resume, and the chatbot will attempt to provide relevant answers.

## Acknowledgement

This project was a guided project, and I appreciate the resources and guidance that helped me create this chatbot.
