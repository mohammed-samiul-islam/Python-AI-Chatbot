# Python AI Chatbot

A small FastAPI web app that sends prompts to a LangChain/LangGraph agent (OpenAI GPT-4) which can read and write text-file notes via natural language.

## Features

- Web UI (Jinja2 template at `templates/index.html`) for submitting prompts
- `POST /agent` endpoint that invokes the agent and returns its response
- Agent tools defined in `agent.py`:
  - `read_note(filepath)` – read the contents of a text file
  - `write_note(filepath, content)` – write content to a text file
- Uses `ChatOpenAI(model="gpt-4", temperature=0.6)`

## Tech Stack

Python · FastAPI · Uvicorn · Jinja2 · LangChain · langchain-openai · LangGraph · python-dotenv

## Project Structure

```
agent.py           # LangChain agent + note tools
main.py            # FastAPI app (GET /, POST /agent), runs Uvicorn on :8000
templates/index.html
requirements.txt
pyproject.toml
```

## Getting Started

```bash
git clone https://github.com/mohammed-samiul-islam/Python-AI-Chatbot.git
cd Python-AI-Chatbot
pip install -r requirements.txt
echo "OPENAI_API_KEY=your_openai_api_key_here" > .env
python main.py
```

Open http://localhost:8000.

### Environment Variables

| Name | Purpose |
|------|---------|
| `OPENAI_API_KEY` | OpenAI API key used by `langchain-openai` |

## Example Prompt

> Please write a new note with title "todo.txt" saying "Finish project README".

The agent calls its `write_note` tool and replies with the result.

## Requirements

- Python 3.8+
- An OpenAI API key

## License

No license file is currently included.
