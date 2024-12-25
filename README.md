# Competitor Analysis Assistant

## Overview

The Competitor Analysis Assistant is a Streamlit-based application that leverages AI agents to perform comprehensive competitor analysis for a given company. The application uses PostgreSQL for data storage and SQLAlchemy as the ORM to manage database interactions.

## Features

- **Competitor Analysis**: Identify key competitors, their strengths, and weaknesses.
- **Market Trends**: Provide detailed information about market trends relevant to the company.
- **Financial Analysis**: Offer detailed financial data about the company.
- **Business Strategy**: Provide detailed business strategy analysis for the company.
- **Data Storage**: Store all generated responses in a PostgreSQL database.

## Requirements

- Python 3.8+
- PostgreSQL
- Streamlit
- SQLAlchemy
- psycopg2-binary
- langchain-core
- langchain-community
- langgraph
- langchain-ollama

## Installation

1. **Clone the repository**:
   ```sh
   git clone https://github.com/yourusername/competitor-analysis-assistant.git
   cd competitor-analysis-assistant
2. **Install the required Python packages:**
   ```sh
   pip install -r requirements.txt  
4. **Set up PostgreSQL:**
5. ```sh
   sudo -u postgres psql
6. **Update the database URL in the code:**
   Open Research_Agent copy.py and update the DATABASE_URL with your PostgreSQL credentials:
   ```sh
   DATABASE_URL = "postgresql+psycopg2://yourusername:yourpassword@localhost:5432/yourdatabase"

## Usage
1. **Run the Streamlit application:**

   Use the application:
   ```sh
      streamlit run Research_Agent.py
   ```
   Enter the company name in the input field.
   Click the "Submit" button to generate the competitor analysis.
   The analysis will be displayed on the interface and stored in the PostgreSQL database

## **PS Note**
This project was made using the Llama 3.1 local LLM. My main focus was to make the agent give a detailed analysis; therefore, the UI is kept simple.
The agentmay get stuck in a Yes/no loop in sometime(for llama3.1 8b model)
