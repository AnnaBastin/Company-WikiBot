# Company-WikiBot
Internal Company Wiki Chatbot built using RAG, that can read internal company documentation and answer queries based on that documentation.

The goal of this project is to build a real-world RAG chatbot entirely inside Google Colab using Python.

The AI assistant can read internal company documents such as:


 • HR policies 
 
 • Company wiki documents
 
 • Internal process documentation
 
 • PDFs and text files
 
 • Convert documents into embeddings
 
 • Store embeddings in a vector database
 
 • Retrieve relevant context based on user questions
 
 • Generate AI-powered answers using Gemini models
 
 

## **Repository Structure**

Company-WikiBot/

 • company.ipynb          # Main Google Colab notebook
 
 • documents/             # Folder containing company documents
 
 • .gitignore
 
 • README.md

 

## **Technologies Used**

 • Python
 
 • Google Colab
 
 • LangChain
 
 • ChromaDB
 
 • Gemini API
 
 • Retrieval-Augmented Generation (RAG)
 
 
## **Features**

 • PDF, TXT, and DOCX document support
 
 • Semantic document retrieval
 
 • Vector database storage using ChromaDB
 
 • AI-generated answers using Gemini
 
 • Modular RAG pipeline
 
 • Runs fully inside Google Colab
 
 • Supported File Types
 

## **The chatbot currently supports:**
 
.txt

.pdf

.docx


## **How It Works :**


Documents are loaded from the documents/ folder

Documents are split into smaller chunks

Gemini embedding models convert text into embeddings

Embeddings are stored in ChromaDB

User questions are matched against relevant document chunks

Gemini generates answers using retrieved context



## **Setup Instructions**


1. Clone the Repository

_git clone https://github.com/AnnaBastin/Company-WikiBot.git_


2. Open the Notebook in Google Colab

Open:

company.ipynb inside Google Colab.

**Google API Key Setup**

This project requires a Google Gemini API key.

Step 1 — Create a Google API Key

Generate a new API key.

Step 2 — Add the API Key to Colab Secrets

Inside Google Colab add the name as GOOGLE_API_KEY	and your api key as the value for it

Enable Notebook Access

Step 3 — Run the Notebook

Run all notebook cells from top to bottom.


## **Important Security Notes**
Never hardcode API keys inside notebook cells

Never upload .env files or API keys to GitHub

The repository uses .gitignore to prevent accidental secret uploads

Example Query

What is the company's remote work policy?

The chatbot retrieves relevant document chunks and generates an AI-powered response based on the internal documentation.


