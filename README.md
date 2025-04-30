# n8n_workflows
A collection of n8n workflows for automation, data manipulation, AI integration, and seamless orchestration with tools like Google Drive, Google Sheets, and LLMs.
# 📧 Automated Email Generator Workflow (n8n + Google Drive + Google Sheets)

This repository contains an **n8n workflow** that reads user data from an Excel file stored in **Google Drive**, extracts relevant information, generates email addresses, and updates a **Google Sheet** with the result.

! Workflow Diagram
![image](https://github.com/user-attachments/assets/ee2430a8-bad8-48c1-b32e-c8ff1173a11c)



## 🚀 Features

- 🔗 Integrates with **Google Drive** to access `.xlsx` files
- 📊 Extracts and parses Excel content dynamically
- 🧠 Extracts the **Name** and **first 3 digits** of the **Social Number**
- ✉️ Generates structured email addresses (e.g., `john.doe123@example.com`)
- 📤 Updates a Google Sheet with the results
- 🧩 Easily extendable for future AI/chatbot applications

## 🧩 Workflow Overview

| Node | Purpose |
|------|---------|
| 🖱️ Manual Trigger | Starts the workflow manually for testing |
| 📂 Google Drive | Downloads the target `.xlsx` file |
| 📄 Extract from File | Parses the Excel content |
| 🔢 Create Row Index | Indexes rows for iteration |
| 🔍 Extract Exact Cell | Gets values from the 'Name' and 'Social Number' columns |
| 💻 Generate Emails | Uses a Function node to generate emails |
| 🧬 Merge Results | Combines generated emails with original data |
| 📑 Google Sheets | Updates a Google Sheet with the final output |

## 📝 Example Input (Excel)

| Name        | Social Number |
|-------------|----------------|
| John Doe    | 123456789      |
| Alice Smith | 987654321      |

## ✉️ Output

| Name        | Social Number | Email                      |
|-------------|----------------|----------------------------|
| John Doe    | 123456789      | john.doe123@example.com    |
| Alice Smith | 987654321      | alice.smith987@example.com |


## ✅ How to Use

1. Import the JSON workflow into your n8n instance.
2. Connect your **Google Drive** and **Google Sheets** credentials.
3. Point to your `.xlsx` file and target sheet.
4. Run the workflow manually or schedule it at your own.
5. Review the updated Google Sheet for email outputs.

## 🔮 Future Plans

- 💬 Build an **AI chatbot** linked to a **vector database** (e.g., ChromaDB, Pinecone)
- 🧠 Allow users to ask for email addresses using natural language queries
- 🔗 Connect to **OpenAI** or **LangChain** for enhanced intelligence

## 🙋‍♂️ Author

**Mirto Gasparinatou** – [GitHub Profile](github.com/mirtogaspar)
                         [LinkedIn Profile] (linkedin.com/in/mirto-m-gasparinatou)

> Found this helpful? Feel free to ⭐️ this repo and share feedback!


