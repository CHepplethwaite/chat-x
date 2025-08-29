Chat-X 🤖 (RAG with Django, DRF, OpenAI & LangChain)

Chat-X is an ongoing Django project that uses OpenAI and LangChain to build a Retrieval-Augmented Generation (RAG) chatbot.

It consists of:

Backend: Django + Django REST Framework (DRF) serving APIs

Frontend: Angular SPA (fe/ folder) for interacting with the chatbot

In simple terms:
This chatbot can read documents, remember them, and answer questions using AI with context from your data — served through a web frontend.

✨ Features (planned)

Upload documents (PDFs, text, etc.)

Store document knowledge in a vector database

Ask natural language questions through a chat page

Get AI answers grounded in your documents (not just guesses)

Frontend consumes DRF APIs for chat, user management, and document handling

🛠️ Requirements

Backend:

Python 3.9+

Django 5.2+

Django REST Framework

LangChain

OpenAI account & API key

Git

Frontend:

Node.js 18+

npm or Yarn

Angular CLI

🚀 Getting Started
1. Clone the project
git clone https://github.com/CHepplethwaite/chat-x.git
cd chat-x

2. Backend Setup (Django + DRF)
python -m venv .venv
.\.venv\Scripts\Activate
pip install -r requirements.txt


Add your OpenAI key:
Create a .env file in the project root:

OPENAI_API_KEY=sk-your-key-here


Apply migrations and run the server:

python manage.py migrate
python manage.py runserver


Backend API base URL will be available at:

http://127.0.0.1:8000/api/

3. Frontend Setup (Angular SPA)
cd fe
npm install
ng serve


Frontend runs at:

http://localhost:4200


Update API URLs in src/environments/environment.ts to point to Django DRF endpoints.

💬 Testing the Chatbot

Currently, you can test the chatbot by asking questions:

"What does the document say about climate change?"


The workflow:

Search document knowledge via DRF API

Pick relevant text

Generate AI answer with OpenAI via LangChain

🤝 How to Contribute

We welcome contributions! You can help by:

Writing Django/DRF code

Adding document loaders and vector stores

Integrating Angular frontend components

Improving UX/UI for chat and uploads

Updating docs and examples

Steps:

Fork the repo

Create a branch

Make changes

Open a Pull Request

📢 Open Invitation

This is an open-source, community-driven project.
Beginners and experts are welcome. Learn and contribute to Django, DRF, Angular, LangChain, and AI chatbots.

Let’s build Chat-X together 🚀

Made with ❤️ using Django + DRF + Angular + OpenAI + LangChain