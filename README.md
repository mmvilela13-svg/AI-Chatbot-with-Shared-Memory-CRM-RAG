# AI-Chatbot-with-Shared-Memory-CRM-RAG
This project implements an AI chatbot that operates across WhatsApp. The system automates customer interactions, document analysis, CRM enrichment, and executive reporting, focusing on real business operations, not demo chatbots.

# Problem

Businesses using multiple messaging platforms often suffer from:
	•	Fragmented conversations
	•	Loss of context when users switch channels
	•	Manual CRM updates
	•	No structured insights from conversations
  

 # Solution

This workflow solves these issues by:
	•	Normalizing messages from multiple channels
	•	Resolving a unified user identity
	•	Persisting conversational memory
	•	Using AI and RAG to analyze messages and documents
	•	Automatically enriching CRM data and notifying stakeholders

# Architecture 

WhatsApp / Instagram
        ↓
Channel Normalization
        ↓
User Identity Resolution
        ↓
Conversation Memory (Redis / DB)
        ↓
AI Reasoning + RAG
        ↓
CRM & Database
        ↓
Management Notifications
