# ConverserAI – A Custom Knowledge Chat Engine

ConverserAI is a powerful AI-driven chatbot solution that allows users to build custom conversational agents by feeding them data from a wide range of sources. Whether it's documents, website content, or video transcriptions, ConverserAI can learn from it all and respond with relevant context.

Designed for developers and organizations seeking a flexible and private AI assistant, the platform comes with secure login integration, modular backend services, and real-time text processing. It combines AI capabilities with practical deployment strategies to deliver a seamless experience.

---

## 🌟 Key Features

• **Multi-Format Knowledge Upload**  
  Train your chatbot using PDFs, articles, notes, and video subtitle files.

• **Smart Authentication System**  
  Uses Google sign-in for quick and secure access to user-specific chat history and configurations.

• **GPT-Driven Responses**  
  Connects with cutting-edge language models for fluid and intelligent dialogue.

• **Fast Contextual Search**  
  Integrates vector databases like FAISS and Pinecone to retrieve contextually similar data efficiently.

• **Language-Agnostic Embedding Support**  
  Uses state-of-the-art embeddings to represent text semantically and store them effectively.

• **File Parsing and Preprocessing**  
  Built-in pipelines using Langchain allow smart text extraction and conversion.

• **Environment-Friendly Architecture**  
  Supports different settings for development, testing, and production with clear separation.

• **Real-Time Task Handling**  
  Manages background processing with Celery using either Redis or AWS SQS.

• **Cloud Storage Ready**  
  Supports scalable file storage using services like AWS S3.

• **Multilingual Foundations**  
  Built with the potential for multi-language interactions and future expansion.

---

## 🛠️ Technologies Used

• **Programming Language**: Python  
• **Backend Framework**: Django REST Framework  
• **Database**: PostgreSQL  

### 📚 Key Libraries

• OpenAI  
• FAISS  
• Pinecone  
• Langchain  
• Celery  
• Django-Allauth  

---

## 📦 Prerequisites

Before setting up, ensure you have:

• Python 3.8 or higher  
• Django 4.1+  
• OpenAI API key  
• Pinecone API key  
• PostgreSQL installed and running  
• Redis or AWS SQS (for asynchronous tasks)

---

## 🚀 Setup Instructions

1. **Clone the project**  
   ```bash
   git clone https://github.com/your-username/converserai.git
   cd converserai
   ```

2. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

3. **Run background workers**  
   ```bash
   celery -A config worker --loglevel=info
   ```

4. **Start the server**  
   ```bash
   python manage.py runserver
   ```

5. **Access the app**  
   Visit `http://127.0.0.1:8000/` in your web browser

---

## 🐧 Linux/macOS Setup Notes

Install required packages if running into environment issues:

```bash
sudo apt install python3-dev libcurl4-openssl-dev gcc libssl-dev -y
pip install --upgrade pip setuptools
pip install pycurl
```

---

## 🌐 Deployment

Deploy your chatbot confidently to Heroku, AWS, or any cloud provider that supports Django and PostgreSQL. Use environment-specific settings for better control and security.

---

## ⚠️ Important Notes

• You do not need `boto3`, `pycurl`, or `django-storages` if you are not using AWS S3 or SQS  
• Make sure your OpenAI and Pinecone keys are set in your environment variables  
• Modify prompt templates and system behavior through the admin interface or config files  

---

## 📈 Future Plans

• Enable integration with messaging apps like Telegram, WhatsApp, and Slack  
• Automatic content summarization and FAQ generation  
• Enhanced conversational memory and better follow-up responses  
• Add support for uploading image and audio content as training sources  
• Build a user analytics dashboard to track usage patterns

---

## 💡 Final Thoughts

ConverserAI bridges the gap between powerful language models and real-world, custom knowledge needs. Whether you are automating support, building a private tutor, or creating a content-aware assistant, this project gives you the building blocks to succeed.

Feel free to fork, enhance, or contribute. Let’s build something intelligent together!

