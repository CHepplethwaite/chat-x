# Chat-X 🤖 (RAG with Django, OpenAI & LangChain)

Chat-X is an **ongoing Django project** that uses **OpenAI** and **LangChain** to build a **Retrieval-Augmented Generation (RAG) chatbot**.  

In simple words:  
This chatbot can read documents, remember them, and use AI to answer questions with context from your data — all served through a Django web app.

---  

This is not finished — it’s a **work in progress** and **open for contributions**.

---

## ✨ Features (planned)
- Upload documents (PDFs, text, etc.)  
- Store document knowledge in a vector database  
- Ask natural language questions through a chat page  
- Get AI answers grounded in your documents (not just guesses)  

---

## 🛠️ Requirements
- Python 3.9+  
- Django  
- LangChain  
- OpenAI account & API key  
- Git  

---

## 🚀 Getting Started

1. **Clone the project**
   ```powershell
   git clone https://github.com/CHepplethwaite/chat-x.git
   cd chat-x
Set up virtual environment

powershell
Copy code
python -m venv .venv
.\.venv\Scripts\Activate
Install dependencies

powershell
Copy code
pip install -r requirements.txt
Add your OpenAI key
Create a file called .env in the project root:

ini
Copy code
OPENAI_API_KEY=sk-your-key-here
Run the server

powershell
Copy code
python manage.py migrate
python manage.py runserver
Visit 👉 http://127.0.0.1:8000/

💬 Testing
Right now the chatbot is basic. Once document ingestion is added, you’ll be able to upload files and ask:

"What does the document say about climate change?"
The chatbot will:

Search your document knowledge.

Pick the most relevant text.

Use OpenAI (via LangChain) to give an answer based on that text.

🤝 How to Contribute
We welcome contributions from everyone!

You can help by:

Writing Django code

Integrating LangChain components

Adding document loaders and vector stores

Designing the chat UI

Improving docs and examples

Steps to contribute
Fork this repo

Create a branch

Make your changes

Open a Pull Request

📢 Open Invitation
This is an open-source, community-driven project.
Beginners and experts are both welcome. If you’re curious about Django, LangChain, or AI chatbots, this is a good project to learn and contribute to.

Let’s build Chatbot-X together 🚀

Made with ❤️ using Django + OpenAI + LangChain