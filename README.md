# Domain-Specific Chatbot using RAG

## Project Overview

This project implements a domain-specific chatbot using Retrieval-Augmented Generation (RAG).
The chatbot answers questions based on information extracted from a specific PDF document.

The system uses LangChain to connect a language model with a vector database containing document embeddings. When a user asks a question, the system retrieves the most relevant text from the document and generates an accurate response.

## Domain

Cybersecurity Basics

The chatbot is trained on a cybersecurity PDF containing explanations of common cyber attacks, security concepts, and defensive techniques.

## Technologies Used

* Python
* LangChain
* ChromaDB (Vector Database)
* HuggingFace Transformers
* Sentence Transformers
* PyPDF

## Project Structure

chatbot_project/

app.py
requirements.txt
README.md
data/
    cybersecurity.pdf

## Setup Instructions

1. Clone or download the project.
2. Install required libraries.

pip install -r requirements.txt

3. Place the domain PDF inside the `data` folder.

4. Run the chatbot.

python app.py

## How the Chatbot Works

1. The PDF document is loaded.
2. The text is split into smaller chunks.
3. Each chunk is converted into embeddings.
4. Embeddings are stored in ChromaDB.
5. When a user asks a question, relevant chunks are retrieved.
6. The language model generates an answer based on retrieved content.

## Example Questions

Q1: What is phishing?
A: Phishing is a cyber attack where attackers trick users into revealing sensitive information through fake emails or websites.

Q2: What is malware?
A: Malware refers to malicious software designed to damage, disrupt, or gain unauthorized access to computer systems.

Q3: What is a firewall?
A: A firewall is a security system that monitors and controls incoming and outgoing network traffic based on security rules.
