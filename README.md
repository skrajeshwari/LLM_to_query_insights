# Leveraging LLMs for Querying Structured Financial Data
The project aims to demonstrate how LLMs can interpret user queries, generate SQL queries, and provide insights dynamically and automatically. The core aim is to integrate LLMs with structured data for dynamically simulating complex query-response flows and generating insights.

Project Flow:
Each query a user makes will follow one of three paths, depending on the nature of the request. The flow is designed to simulate real-world interaction with LLM-driven systems but is tailored to demonstrate how the technology works with structured data.

Path 1:
For Queries Needing Data Access and Insights
These queries require retrieving data from the database, running additional analyses, and summarizing insights.

Steps: LLM generates an SQL query → Retrieves data from the database → Python code for analysis → Insight generation → Suggestions for next steps.

This demonstrates how a LLM dynamically creates SQL queries and generates meaningful outputs from structured data.

Path 2:
For Exploratory or Informational Questions
These queries are more exploratory and don’t require accessing data, like asking about the available dataset or metadata.

Steps: LLM responds directly based on its understanding → It offers suggestions for further exploration.

This demonstrates how to leverage LLMs for general conversation-style queries and data exploration without needing heavy data processing.

Path 3:
For Out-of-Scope or Irrelevant Questions
Queries that are outside the scope of the system (e.g., "What is the weather today?").

Steps: LLM generates a polite response indicating the question is out of scope → Suggests relevant questions within the system’s scope.

Technical Stack:
LLM: Pre-trained large language models (e.g., GPT-4) for query interpretation and code generation.
SQL Database: Storing structured data (e.g., Nifty 50 financial data) that can be queried based on user requests.
Python: Used for data manipulation and analysis (with libraries like pandas), allowing the system to generate insights from the raw data.
APIs/Integrations: Used to create an interface between the LLM, SQL database, and Python execution environment.
