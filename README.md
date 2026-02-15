# Python AI Chatbot

A simple AI-powered chatbot web app built with **FastAPI** that uses a LangChain agent to process prompts and perform note-taking tasks like reading and writing text files based on natural language instructions. :contentReference[oaicite:1]{index=1}

---

## 🚀 Features

- 🧠 Conversational AI powered by **LangChain + OpenAI**  
- 📄 Tools for reading and writing notes via natural language  
- 🌐 Web interface with FastAPI & Jinja2 templates  
- ⚡ Easy to run locally with minimal setup

---

## 🗂️ Project Structure

#### 📦 Python-AI-Chatbot
- agent.py # Defines the AI Agent and tools
- main.py # FastAPI web app
- requirements.txt # Python dependencies
- pyproject.toml # Project metadata
- templates/ # HTML UI templates
- README.md

---

## 🛠️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/mohammed-samiul-islam/Python-AI-Chatbot.git
   cd Python-AI-Chatbot


2. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    
    
3. **Set up environment variables**
    ```bash
    OPENAI_API_KEY=your_openai_api_key_here
    
---

## 📦 Usage
### Run the API
    ```bash
    python main.py
    

This starts the FastAPI server on http://localhost:8000.
You’ll see a simple HTML interface where you can submit prompts to interact with the AI agent.

### How the agent “Thinks”

The LangChain agent can do things like:

- Read the contents of a text file
- Write content to a file
- Respond to natural language prompts

Example tools are already defined in agent.py.

---

## 🧪 Example Prompt

Try sending it something like:
    ```bash
    Please write a new note with title “todo.txt” saying “Finish project README”.

The agent will use its note writing tool and return a helpful response.

---

## 🧠 Requirements

Your project needs:

    - Python 3.8+

    - OpenAI API Key

    - Libraries in requirements.txt, including:

        - FastAPI

        - Uvicorn

        - LangChain

        - LangChain-OpenAI

        - LangGraph

        - python-dotenv

        - Jinja2

---

## 💡 Contribution

Feel free to:

- Improve the frontend UI
- Add more tools for the agent
- Integrate chat history or authentication

---

## 📄 License

This project doesn’t currently include an open license — if you want to make it open source for others to use, consider adding a LICENSE file.

--- 

## 🙌 Acknowledgements

Thanks for building and sharing this repository — a great base for learning about building AI-assisted web apps with FastAPI and LangChain! 🎉

---