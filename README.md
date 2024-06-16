# Llama-3 Chatbot

Welcome to the Llama-3 Chatbot project! This chatbot allows you to interact with the Llama-3 model via a simple command-line interface. Type your messages, and receive responses from Llama-3.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Resources](#resources)
- [License](#license)

## Installation

### Prerequisites

- Python 3.8 or higher
- `ollama` library
- Downlaod and install `ollama` from the official website as per your operating system: https://ollama.com/download/windows

### Llama-3 setup
- Open the terminal and change the directory where Ollama is located (C:OS drive)
- Download the llama3 model on the local system
  ```sh
  ollama pull llama3
  ```
- Lists all the models downloaded in the local system (4.7 GB)
  ```sh
  ollama list
  ```
- Run the model
  ```sh
  ollama run llama3:latest
  ```
- Serving llama locally
  ```sh
  ollama serve
  ```
  
### Steps

1. Clone the repository:
    ```sh
    git clone https://github.com/anushkaspatil/llama3-chatbot.git
    cd llama3-chatbot
    ```

2. Create a virtual environment (optional but recommended):
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required Python packages:
    ```sh
    pip install ollama
    ```
    

## Usage

You can choose between two methods to run the chatbot: synchronous and asynchronous.

### Synchronous Method

The synchronous method is straightforward is slower due to the blocking calls.
To start the chat with the synchronous method, install and import the dependencies and run the file chat.py

#### Features

- Real-time streaming of responses from the Llama model
- Infinite loop for continuous interaction

1. **Run the chatbot**:
  ```sh
  python chat.py
  ```
2. **Interact with the chatbot**:
    - Enter your messages when prompted.
    - The chatbot will provide responses from the Llama model.
  
### Asynchronous Method

This method streams responses from a Llama model using the `AsyncClient`. The chatbot continuously prompts the user for input and streams the responses in real-time.
`AsyncClient` from Ollama is required.

#### Features

- Asynchronous operation using `asyncio`
- Real-time streaming of responses from the Llama model
- Infinite loop for continuous interaction

1. **Run the chatbot**:
    ```bash
    python updated_chat.py
    ```

2. **Interact with the chatbot**:
    - Enter your messages when prompted.
    - The chatbot will stream responses from the Llama model.
  
By following these steps and guidelines, you'll be well-equipped to embark on your LLM journey using Llama-3. Happy coding!


## **Examples**
These are a few screenshotes attached of the working chatbot for reference.

1.
![Screenshot (312)](https://github.com/anushkaspatil/llama3-chatbot/assets/103093836/569693d1-b0fe-4f12-ada2-04ec8b5149d8)



2.
![Screenshot (311)](https://github.com/anushkaspatil/llama3-chatbot/assets/103093836/ba3c156b-6d13-47d3-b7e0-37965433e6fb)


## **Resources**
1. [Official Doucumentation Meta Llama](https://llama.meta.com/docs/get-started/)
2. [Reference Article - Beginner Friendly](https://www.datacamp.com/tutorial/run-llama-3-locally)
3. [YouTube video - 1st half](https://www.youtube.com/watch?v=uxXxXaMpn4M&t=498s)
   

## **License**
This project is licensed under the [MIT License](LICENSE).



