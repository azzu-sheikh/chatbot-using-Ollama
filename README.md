# chatbot-using-Ollama
# AI Chatbot with History

***This project is an AI chatbot built using Streamlit and Langchain. The chatbot is designed to assist 5th grade students by providing brief and helpful explanations. The chatbot maintains a history of the conversation, allowing users to see previous interactions.***

## Features

- AI chatbot that provides brief and helpful explanations.
- Maintains a history of the conversation.
- Built using Streamlit for the web interface.
- Utilizes Langchain for the chatbot model and prompts.

## Installation

1. **Clone the repository:**
git clone https://github.com/azzu-sheikh/chatbot-using-Ollama

2. **Install the required dependencies:**
   ollama run llama3.2:1b

 pip install -qU langchain-ollama
 
 pip install langchain
 
 pip install streamlit

3. **Ensure you have the necessary model running locally.**
   The chatbot uses the llama3.2:1b model from Langchain, which should be accessible at http://localhost:11434/.

**Usage**
1. Run the Streamlit application:
      "python streamlit run chatbot_with_history.py"

2. Open your web browser and go to http://localhost:8501 to interact with the chatbot.

## Code Overview

Imports: The script imports necessary modules from Streamlit and Langchain.

Title and Header: Sets the title and header of the Streamlit app.

Model Initialization: Initializes the ChatOllama model with the specified base URL.

System Message: Defines the system message prompt template.

Chat History: Initializes the chat history in the session state if it doesn't exist.

Form: Creates a form for user input.

Generate Response: Defines a function to generate responses from the model.

Get History: Defines a function to retrieve the chat history.

Submit Handling: Handles the form submission, generates a response, and updates the chat history.

Display Chat History: Displays the chat history in the Streamlit app.

## Example
Enter your question in the text area and click "Submit".

The chatbot will generate a response and display it along with the chat history.
