# Chatbot Project

This project is a simple command-line chatbot that leverages OpenAI's GPT-4 API to generate responses. It continuously prompts the user for input, sends the text to the GPT-4 model, and displays the generated response in the terminal. This repository serves as a basic template for integrating OpenAI's language models into your own projects.

## Project Overview

- **Purpose:**  
  Demonstrates how to set up and interact with OpenAI's API using Python. It provides a straightforward example of continuously taking user input, processing it via the GPT-4 model, and outputting the chatbot's response.

- **Key Features:**  
  - Loads environment variables from a `.env` file.
  - Initializes an OpenAI client with an API key.
  - Implements a simple interactive loop that accepts user messages until the command "exit" is given.
  - Acts as a foundation for building more complex conversational AI applications.

## Setup and Installation

1. **Clone the Repository:**  
   Clone this repository to your local machine using:
   ```
   git clone https://github.com/rafaelVictor05/Chatbot.git
   ```

2. **Install Dependencies:**
    Make sure you have Python installed, then install the required packages:
    ```
    pip install python-dotenv openai
    ```

3. **Configure Environment Variables:**
    Copy the .env.example file and rename the copy to .env.
    Open the .env file and paste your API key into the API_KEY variable.
    For example, your .env file should look like:
    ```
    API_KEY=your_openai_api_key_here
    ```
4. **How It Works**

**Environment Setup:**
The script uses the python-dotenv package to load environment variables from the .env file. This is where your OpenAI API key is stored securely.

**Initializing the OpenAI Client:**
After retrieving the API key, the script initializes an instance of the OpenAI client. This client is used to make API calls to generate responses.

**Chatbot Functionality:**
The main() function:

Continuously prompts the user for input.

Processes the input using the generate_response() function which sends the text to the GPT-4 model.

Displays the chatbot's response.

Ends the conversation when the user types "exit".

Running the Project
To start the chatbot, simply run the script with:
    ```
    python <your_script_name>.py
    ```

