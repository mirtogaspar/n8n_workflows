# Project: Automated Email Management with Pinecone and n8n

## Workflow Description
The workflow consists of two main agents:

1. **mail_agent_pinecone**: This agent is responsible for automatically sending emails. It behaves as a tool, utilizing n8n to streamline the email dispatch process.
![Agent](https://github.com/user-attachments/assets/fa12aae5-23f7-4d7f-849b-2d9c10a60284)


3. **send_mail_tool**: This agent retrieves emails from the Pinecone vector store and sends them. It leverages semantic retrieval capabilities to ensure relevant email content is accessed and dispatched efficiently.
![sendmail_agent](https://github.com/user-attachments/assets/fd64b4d2-8316-4dfa-b8eb-8a6583b2a41b)


## Components
- **Manual Trigger**: Initiates the workflow manually for testing purposes.
- **Pinecone Vector Store**: Used for storing email content in a vector format, enabling semantic search and retrieval.
- **Embeddings OpenAI**: Generates embeddings for the email content to facilitate semantic search.
- **Google Drive**: Integrates with Google Drive to download and upload documents.
- **Google Docs**: Updates and retrieves content from Google Docs.
- **Google Sheets**: Reads data from Google Sheets.
- **Recursive Character Text Splitter**: Splits text into manageable chunks for processing.
- **Memory Buffer**: Temporarily stores data during processing to ensure smooth workflow execution.
- **Code Nodes**: Custom JavaScript code for processing and combining email content.

## Setup Instructions
1. Clone the repository.
2. Install n8n and configure the necessary nodes.
3. Replace the placeholder API keys in the workflow with your actual keys.
4. Run the workflow to test the email automation and retrieval process.

## Usage
- **Email Sending Agent**: Automatically sends emails based on predefined triggers and conditions.
- **Email Retrieval Agent**: Retrieves and sends emails from the Pinecone vector store using semantic search.


