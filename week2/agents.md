# Agents
## Introduction
The typical RAG flow is a rigid process and determistic: given a user input, we query the search engine for relevant documents, and use the search results to build a context-aware LLM prompt.

Agentic RAG, there is no such fixed structure. Instead of imposing a systematic search for every user query, the agent has at its disposal a search tool, which it may turn to __if required__. There is a decision by the agent to invoke the tool, and a single user query may lead to multiple engine searches.

Agents are configured using instructions:
- how the agent should help the user
- which tool it has at its disposal

Agentic RAG offers a wider range of possibilites for helping users, and makes for an autonomous system.