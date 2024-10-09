# Chatbot-with-OpenAI-and-Ollama
Project Overview
This project implements two AI-powered chatbots using different language models: one utilizing OpenAI's GPT models and another using open-source models via Ollama. The chatbots are designed to answer user queries in a conversational manner, demonstrating the capabilities of both proprietary and open-source language models.
Features
Two separate chatbot implementations: OpenAI and Ollama
User-friendly interface built with Streamlit
Customizable model selection and response parameters
Integration with LangChain for enhanced language model interactions
Technologies Used
Python
Streamlit
LangChain
OpenAI API
Ollama
dotenv for environment variable management
Implementation Details
OpenAI Chatbot (app_OpenAI.py)
Utilizes OpenAI's GPT models (gpt-4, gpt-4-turbo, gpt-4)
Requires an OpenAI API key for authentication
Allows users to select the model and adjust temperature and max tokens
Ollama Chatbot (app_Ollama.py)
Uses open-source models (gemma:2b, llama3) via Ollama
Does not require an API key
Provides options to select the model and adjust temperature and max tokens
Common Features
Both implementations use a consistent prompt template
Responses are generated using LangChain's ChatPromptTemplate and StrOutputParser
LangSmith tracking is enabled for performance monitoring
How It Works
Users input their query in the Streamlit interface
The selected model (OpenAI or Ollama) processes the query
The chatbot generates a response based on the input and selected parameters
The response is displayed to the user
Setup and Running
Install dependencies: pip install -r requirements.txt
Set up environment variables (for OpenAI API key)
Run the OpenAI chatbot: streamlit run app_OpenAI.py
Run the Ollama chatbot: streamlit run app_Ollama.py
