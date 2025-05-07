📬 Email Vectorization Pipeline
This phase of the project focuses on extending functionality by storing generated email content in a Pinecone vector store for semantic retrieval using Large Language Models (LLMs).

🧠 Overview
Continuing from the previous stage where emails were generated in the generate_emails module, this process performs the following steps:

Extracts the specific spreadsheet cells that contain the contact names and the generated email content.

Creates a Google Sheets document to organize and store the extracted data.

Uploads the document contents into Pinecone, where the data is vectorized for intelligent retrieval.

This enables LLM-powered agents to search and retrieve emails based on natural language queries.


⚙️ Workflow
Data Extraction: Download from Google drive and read the Google sheet using Google Sheets API.

Parses the data structure output by generate_emails.

Isolates relevant fields (e.g., columns: Name, Email).

Google Sheet Creation

Initializes a new Google Sheet using the Google Sheets API.

Populates it with the name-email pairs.

Optionally configures access and formatting.

Pinecone Upload

Connects to an existing Pinecone index.

Converts email text into embeddings using an OpenAI model.

Uploads the vectors along with metadata (e.g., name, content tags) into Pinecone.

📌 Purpose
This step makes it possible to:

Perform semantic search over generated emails.

Enable context-aware memory for LLM agents.

Support retrieval-augmented generation (RAG) applications.
