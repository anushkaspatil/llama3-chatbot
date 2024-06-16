# Llama-3 Chatbot

Welcome to the Llama-3 Chatbot project! This chatbot allows you to interact with the Llama-3 model via a simple command-line interface. Type your messages, and receive responses from Llama-3.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

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
  

### Steps

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/llama3-chatbot.git
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

The synchronous method is straightforward but might be slower due to blocking calls.

To start the chat with the synchronous method, run:

```sh
python sync_chatbot.py

llama3-chatbot/
│
├── async_chatbot.py    # Asynchronous chatbot implementation
├── sync_chatbot.py     # Synchronous chatbot implementation
├── README.md           # Project README file
├── LICENSE             # Project license file
├── venv/               # Virtual environment directory (optional)
│
└── requirements.txt    # Required Python packages

