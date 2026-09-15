# AI Agent Automation Workflows (n8n)

Two integrated automation flows built in n8n:

## 1. Lead Intake & Trust Classification
Form submission → validates sender domain (gmail.com check) → 
LLM (OpenAI) tags/classifies the submission → logs to a data table.

## 2. RAG-based Chat Agent
Google Drive trigger → downloads doc → chunks & embeds via 
Google Gemini embeddings → stores in Pinecone vector DB → 
AI Agent (Gemini) answers chat queries using retrieved context, 
with memory across the conversation.

**Tools:** n8n, OpenAI API, Google Gemini API, Pinecone, LangChain nodes

