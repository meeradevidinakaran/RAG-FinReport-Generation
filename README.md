# RAG-FinReport-Generation
This is a RAG Workflow designed to generate financial report based on the company data available and also sends this report to desired email recipients.  

# Background
At NovaCart, the Product Finance team is responsible for delivering a high-stakes monthly analysis that dictates strategic direction. Each month, the team must synthesize internal product performance metrics with complex external market data, including industry outlooks and shifting consumer behavior.

Currently, this process requires manual data aggregation and cross-referencing between internal databases and external intelligence reports, which can be time-consuming and prone to oversight.

# Goal
The primary objective is to generate a comprehensive Monthly Financial Standing Report by the 1st of every month. This report must provide leadership with a clear, data-driven snapshot of NovaCart’s performance relative to the broader market, enabling them to make faster and more informed strategic decisions.

# Solution
We will be using the n8n platform for building the workflow ; Pinecone for Vector db ; Cohere for re ranking and Open AI LLM models.

This RAG Workflow should have an AI Finance Reporting Agent that is capable of autonomous data synthesis and insight generation. 

The agent will:
● Query internal data: Access and analyze real-time product sales numbers stored in a Vector Database created as part of the **internal data Ingestion Pipeline**.

● Analyze external trends: Scan and interpret industry outlooks and consumer behavior reports from designated Knowledge Sources. This is as well stored in a different index on the same vector data base as **extenral data Ingestion.**

● Synthesize & Report: Correlate internal performance with external market conditions to produce a structured summary for leadership and Report over Email: Send the final monthly report over email to the required stakeholder. As part of the **Retrieval Pipeline.**

# System Design
assets/RAG_FinReport.png

# Scaling_Strategy
docs/Scaling_Strategy.md

# Setup Instructions
docs/Setup_Instructions.md

# Demo 
