# Simple GPT-4 Chatbot

This project provides a simple command-line interface for interacting with OpenAI's GPT-4 model. It references previous messages to continue conversations.

## Prerequisites

- Python 3.6 or higher
- OpenAI Python library: Install using `pip install openai`.
  - If this doesn't work, try `pip3 install openai`
- pyreadline Python library: Install using `pip install pyreadline`.
  - If this doesn't work, try `pip3 install pyreadline`
- OpenAI API key (and access to GPT-4)

## Setup

1. Clone this repository or copy the code into a new file named `chattyCLI.py`.
2. Obtain an API key from OpenAI and replace `<API key>` in the `chattyCLI.py` code with your API key.

## Usage

1. Run the chatbot script in your terminal with the command `python chattyCLI.py`. If this doesn't work, try `python3 chatty.py`.
2. Type your questions or statements and press Enter to get a response from the AI.
3. To end the conversation, type `q` and press Enter.
4. The chatbot conversation will be saved as a markdown file named `chat_output_<current date and time>.md` on your desktop.

## How it works

- The script uses OpenAI's GPT-4 to generate responses based on user input.
- AI references previous messages within the same session.
- An animated spinner appears while pending the AI response.
- When the user inputs `q` to quit, the conversation saves to a markdown file on the user's desktop.

## FAQ

Q: How do I view a markdown file?

A: Download Visual Code Studio. Launch the markdown file and click the `Open Preview to the Side` button. A more readable format should appear in the right pane.

## Tinkering Notes

Adjust values according to your preferences.

By default, `max_tokens=1500` and `temperature=1`.
