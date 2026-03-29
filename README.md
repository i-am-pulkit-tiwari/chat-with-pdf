# Chat with PDF

AI-powered PDF reader built with LangChain and Streamlit. Upload PDFs and chat with your documents using natural language.

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=Streamlit&logoColor=white)](https://streamlit.io)
[![LangChain](https://img.shields.io/badge/LangChain-121212?logo=langchain&logoColor=white)](https://langchain.com)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)

## Features

- **RAG-based Q&A** - Get accurate answers using Retrieval-Augmented Generation
- **Source Citations** - See exactly which parts of the PDF were used to answer
- **Interactive UI** - Clean Streamlit interface for easy document interaction
- **Multi-PDF Support** - Chat with multiple documents simultaneously
- **Persistent Chat History** - Conversation context is maintained throughout the session

## Use Cases

- Research paper analysis
- Legal document review
- Contract summarization
- Quick insights from reports and manuals

## Tech Stack

| Component | Technology |
|-----------|------------|
| Framework | [Streamlit](https://streamlit.io) |
| LLM Orchestration | [LangChain](https://langchain.com) |
| LLM | [Groq](https://groq.com) (OpenAI-compatible) |
| Embeddings | HuggingFace (thenlper/gte-small) |
| Vector Store | ChromaDB |
| PDF Processing | PyPDF2, PyPDFLoader |

## Prerequisites

- Python 3.8+
- Groq API key

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/i-am-pulkit-tiwari/chat-with-pdf.git
   cd chat-with-pdf
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up your API keys:
   ```bash
   export OPENAI_API_KEY="your-api-key-here"
   ```

## Usage

Run the Streamlit app:

```bash
streamlit run app.py
```

Then open your browser to `http://localhost:8501` and:
1. Upload your PDF(s)
2. Wait for processing to complete
3. Start asking questions in natural language

## Configuration

Create a `.env` file for local configuration:

```env
GROQ_API_KEY=your_key_here
```

Or set it as an environment variable:
```bash
export GROQ_API_KEY="your-api-key-here"
```

## Project Structure

```
chat-with-pdf/
├── app.py                 # Main Streamlit application
├── htmlTemplates.py       # Chat UI templates (CSS, message templates)
├── requirements.txt       # Python dependencies
├── .github/profile/       # GitHub profile README
├── LICENSE               # GPL v3 License
├── README.md             # This file
└── img_1.png             # Demo screenshot
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.


## PREVIEW

Screenshot of the interactive PDF chat interface:

![Chat with PDF Demo Screenshot](img_1.png)