# StockAI-Approach

A minimalist implementation showing how to bridge a Trading API with a Large Language Model (LLM).

## Core Approach
The project follows a linear pipeline:
1. **Data Ingestion**: Fetch live portfolio data (Public.com) and market news (Yahoo Finance).
2. **Context Injection**: Pass raw financial data into a prompt template for Google Gemini.
3. **Sentiment Analysis**: AI evaluates data to determine a Buy/Hold/Sell rating.
4. **Automated Feedback**: Results are displayed via a Streamlit UI and sent to the user via an SMS Gateway.

## Execution Flow
- `app.py`: Entry point for the Web UI.
- `main.py`: Orchestrates the data flow between services and the AI.
- `brain.py`: Manages the LLM logic and prompt engineering.
- `Services/`: Modular scripts for API connections and notifications.

## Key Dependencies
- `streamlit`: For the dashboard.
- `langchain-google-genai`: For AI logic.
- `requests`: For API communication.
