# Natural-Language-Data-Analysis-using-n8n-Ollama-MySQL

This repository contains an n8n workflow designed to automate the processing of incoming chat messages using the Ollama language model and execute a custom MySQL query based on the processed data. The workflow is ideal for applications such as chatbots, customer service automation, or any system requiring real-time processing of chat-based inputs with database integration.

## Tech Stack

- n8n — Workflow automation (Chat Trigger, Basic LLM Chain, MySQL nodes)

- Ollama — Local LLM for SQL generation

- MySQL — Relational database


## Workflow Overview

### The workflow consists of three main nodes:


- **Trigger Node:** Activates when a chat message is received.

- **Basic LLM Chain:** Processes the chat message using the Ollama language model.

- **MySQL Node:** Executes a custom MySQL query based on the output from the language model.


## The workflow follows this sequence:

- **Trigger:** Starts when a chat message is received via the "When chat message received" node.

- **Processing:** The message is passed to the "Basic LLM Chain" node, which uses the Ollama model to process the input.

- **Action:** The processed data is used by the "MySQL1 executeQuery" node to perform a database operation (e.g., storing results, updating records, or retrieving data).

