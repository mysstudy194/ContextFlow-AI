# ContextFlow AI 🤖

**An AI-powered conversational chatbot built with Python and Groq API, featuring LLM integration, conversation memory, automatic message summarization, streaming responses, and token usage monitoring.**

## 📌 About The Project

ContextFlow AI is a Python-based conversational chatbot that uses Large Language Models (LLMs) through the Groq API.

The chatbot maintains conversation history, generates real-time streaming responses, and periodically summarizes earlier conversations to help manage context.

It also uses Hugging Face Transformers for tokenization and includes token usage and estimated cost tracking.

## ✨ Features

- **LLM Integration:** Connects to Groq API using the OpenAI Python SDK.
- **Conversation Memory:** Maintains chat history using message roles (system, user, and assistant).
- **Automatic Summarization:** Summarizes earlier conversation messages after every five iterations.
- **Streaming Responses:** Displays AI responses gradually instead of waiting for the complete response.
- **Tokenization:** Uses Hugging Face AutoTokenizer with Llama 3.1 8B.
- **Prompt Length Validation:** Restricts user prompts to a maximum of 10 tokens.
- **Token Usage Monitoring:** Tracks input, output, and total token usage when usage data is returned.
- **Cost Estimation:** Calculates estimated API costs using configured input and output rates.
- **Interactive Chat:** Supports continuous conversations through a command-line interface.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Groq API | LLM inference |
| OpenAI SDK | API communication |
| Hugging Face Transformers | Tokenization |
| Llama 3.1 8B | Tokenizer |
| GPT-OSS-20B | Chat and summarization model |
| Python-dotenv | Environment variable management |

## ⚙️ Project Structure

```text
ContextFlow-AI/
│
├── chat_bot.py
├── .env
├── .gitignore
├── requirements.txt
└── README.md
```

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/ContextFlow-AI.git
```

### 2. Navigate to Project Directory

```bash
cd ContextFlow-AI
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it:

**Windows:**
```bash
venv\Scripts\activate
```

**Linux / macOS:**
```bash
source venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install openai python-dotenv transformers
```

### 5. Configure Environment Variables

Create a `.env` file in the project directory:

```env
GROQ_API_KEY=your_groq_api_key
```

Get your API key from [Groq Console](https://console.groq.com/keys).

### 6. Run the Project

```bash
python chat_bot.py
```

## 🧠 How It Works

1. The chatbot initializes a connection with the Groq API.
2. A system message defines the chatbot's behavior and identity.
3. The user enters a prompt through the terminal.
4. Hugging Face Tokenizer checks the prompt length.
5. The conversation history is sent to the LLM.
6. The LLM generates a response using streaming.
7. The chatbot displays the response in real time.
8. Conversation messages are stored in memory.
9. After every five iterations, earlier messages are summarized.
10. Token usage and estimated API cost are displayed in the final report.

## 💡 Key Concepts Implemented

- Large Language Model (LLM) Integration
- Prompt Engineering
- Conversation History Management
- Context Summarization
- Streaming Generation
- Tokenization
- Token Usage Monitoring
- Environment Variable Management
- Python Object-Oriented Programming (OOP)
  
⭐ If you find this project interesting, consider giving it a star!

👨‍💻 Author
Muhammad Talha Abid




