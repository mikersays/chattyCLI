# Simple GPT-4 Chatbot

This project provides a simple command-line interface for interacting with OpenAI's GPT-4 model. It includes a spinning cursor animation to indicate that the AI is processing your input and saves the conversation to a text file on your desktop.

## Prerequisites

- Python 3.6 or higher
- OpenAI Python library: Install using `pip install openai`

## Setup

1. Clone this repository or copy the code into a new file named `chatty.py`.
2. Obtain an API key from OpenAI and replace `<API token>` in the code with your API key.
3. If needed, replace `"gpt-4"` in the `generate_response` function with the appropriate model name.

## Usage

1. Run the chatbot script in your terminal with the command `python chatty.py`.
2. Start typing your questions or statements and press Enter to get a response from the AI.
3. To end the conversation, type `quit` and press Enter.
4. The chatbot conversation will be saved as a text file named `chat_output_<current date and time>.txt` on your desktop.

## How it works

- The script uses OpenAI's GPT-4 to generate responses based on user input.
- The spinning cursor is implemented using a separate thread that displays an animated spinner while waiting for the GPT-4 response.
- The conversation is saved to a text file on the user's desktop with a timestamp to ensure unique filenames for each session.