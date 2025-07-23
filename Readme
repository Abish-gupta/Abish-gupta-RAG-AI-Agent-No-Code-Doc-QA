# RAG AI Agent: No-Code Business Document Q&A System

## Overview

This project is a no-code RAG (Retrieval-Augmented Generation) AI agent that automates document search and Q&A. Built with n8n, OpenAI, Cohere, Supabase, and Google Drive integration, it enables teams to query business documents in natural language with live responses and full source traceability.

## Business Use Case
Automate knowledge management for teams by ingesting, chunking, and indexing documents from Google Drive to a secure vector database. Reduce manual document search time and enable real-time, context-aware Q&A through chat or integrated tools like Slack.

## Tech Stack
- n8n (Workflow Automation)
- OpenAI (Embedding & LLM)
- Cohere (Reranking)
- Supabase (Vector Store)
- Google Drive (Document Source)
- Slack (Chat Integration, optional)

## Key Features
- Automated document ingestion from Google Drive
- Intelligent document chunking and vector storage
- Semantic search with context-aware Q&A
- Source-cited answers with full metadata tracking
- Automated cleanup for deleted files
- Modular, no-code automation (powered by n8n)

## Workflow

1. **Trigger**: Scheduled or manual workflow start.
2. **Document Fetch**: Syncs files from a designated Google Drive folder.
3. **Processing**: Splits text into overlapping chunks (750 chars), generates embeddings using OpenAI API.
4. **Storage**: Stores chunks and embeddings in Supabase.
5. **Q&A Flow**: On user question, finds relevant chunks via vector search, reranks results using Cohere, and generates a sourced answer with OpenAI.
6. **Cleanup Module**: Periodically identifies and removes embeddings for deleted files in Google Drive.

## Credential Setup
- **Supabase**: Host, service key, and project URL
- **OpenAI**: API key 
- **Cohere**: API key for reranking 
- **Google Drive**: OAuth or service account setup for API access 

## Table Structure
- `documents` table: Stores each chunk and its vector embedding.
- `documents_metadata` table: Tracks original file, upload time, and document attributes.

## Example Use Case
**Scenario:**  
A team uploads project reports to Google Drive. A team member asks, “What are the main deliverables in the Q3 report?”  
The agent retrieves, reranks, and cites the relevant Q3 doc’s section, responding instantly in Slack or chat.




