# Byte – Multi-Turn AI Programming Mentor

Byte is a beginner-friendly AI programming mentor chatbot built using Python, FastAPI, Groq LLM API, and SQLite. It is designed to help beginners understand programming concepts through simple explanations and conversational interactions.

## Features

- **AI-powered responses:** Uses a Groq-hosted language model to answer programming questions.
- **Multi-turn conversations:** Maintains conversation history using unique conversation IDs.
- **Persistent storage:** Stores conversation messages in an SQLite database.
- **Context-window management:** Loads the most recent 10 messages to provide relevant conversation context.
- **FastAPI backend:** Provides a REST API for interacting with the chatbot.
- **Error handling:** Handles API errors and invalid requests.
- **Secure API key management:** Uses environment variables to access the API key.

## Technologies Used

- Python
- FastAPI
- Groq API
- SQLite
- Pydantic
- Uvicorn
- Google Colab

## Project Structure

```text
byte-multiturn-chatbot/
├── Byte_Groq_MultiTurn_Chatbot.ipynb
├── Byte_FastAPI_Backend.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── .env.example
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/byte-multiturn-chatbot.git
cd byte-multiturn-chatbot
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure the API key

Create a `.env` file using `.env.example` as a reference:

```env
GROQ_API_KEY=your_actual_api_key
```

Never upload your actual `.env` file or API key to GitHub.

### 4. Run the notebooks

Open the notebooks in Google Colab:

- `Byte_Groq_MultiTurn_Chatbot.ipynb` – Initial multi-turn chatbot implementation.
- `Byte_FastAPI_Backend.ipynb` – FastAPI backend with SQLite-based conversation storage.

Configure your Groq API key securely using Colab Secrets before running the relevant cells.

## Context Management

Byte maintains conversation history using conversation IDs. It retrieves the most recent 10 messages from SQLite and includes them in the model request, allowing the chatbot to refer to earlier parts of a conversation.

## Future Improvements

- Add a Streamlit or web-based user interface.
- Implement conversation summarization for longer chats.
- Improve conversation management and database handling.
- Deploy the backend as a publicly accessible application.

## Author

Developed as a multi-turn LLM chatbot project.# byte-multiturn-chatbot
