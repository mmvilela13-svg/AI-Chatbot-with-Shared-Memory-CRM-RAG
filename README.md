# Overview

This repository contains an n8n automation workflow for WhatsApp designed to handle customer interactions in a smart, human-like, and fully automated way.

The workflow acts as a WhatsApp chatbot that provides company information using RAG (Retrieval-Augmented Generation) memory, while also keeping the CRM automatically updated.



# Features
	•	Automated WhatsApp Customer Support
	•	Responds to customer inquiries with accurate company information using RAG memory.
	•	CRM Integration
	•	Automatically updates the last contact date of existing customers.
	•	Registers new customers in the CRM when they contact the business for the first time.
	•	Redis Short-Term Memory
	•	Uses Redis as short-term memory to group multiple incoming messages.
	•	Waits 10 seconds to collect consecutive messages before generating a response, improving conversation flow.
	•	Multimodal Message Support
	•	Supports:
	•	Text messages
	•	Voice messages
	•	Images
	•	Document analysis
	•	Humanized Responses
	•	Splits responses into up to 3 natural messages when needed.
	•	Ensures responses feel conversational and human, rather than robotic.


# How It Works (High Level)
	1.	Receives WhatsApp messages via webhook.
	2.	Temporarily stores messages in Redis to group them.
	3.	Processes user intent and retrieves relevant information using RAG.
	4.	Updates or creates customer records in the CRM.
	5.	Sends structured, human-like responses back to the user.



# Requirements
	•	n8n
	•	WhatsApp API provider (e.g. WAHA or similar)
	•	Redis instance
	•	CRM system
	•	Proper credentials configured for each service

# Important:
For this workflow to work correctly, each service must use its own credentials.



# Use Cases
	•	Automated customer support via WhatsApp
	•	Lead registration and CRM updates
	•	Multimodal customer interaction (voice, images, documents)
	•	Human-like conversational AI for businesses