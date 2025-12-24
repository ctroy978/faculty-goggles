# Product Guide: Teaching Assistant Agent

## Initial Concept
A teaching assistant agent designed to automate educational tasks such as creating reading handouts and evaluating papers. The agent acts as a coordinator for a suite of FastMCP servers, each dedicated to a specific function.

## Core Value Proposition
- **Modular Efficiency:** Leverages specialized MCP servers (like `latextMCP`) for distinct tasks, allowing for scalable and maintainable feature growth.
- **Streamlined Workflow:** Automates the complex process of generating high-quality educational materials (e.g., LaTeX-based handouts) through a unified interface.
- **Teacher-Centric:** Provides an intuitive chat-based interface for teachers to interact with powerful backend tools without needing technical expertise.

## Target Audience
- **Primary:** Teachers and educators looking to automate administrative and content-creation tasks.
- **Secondary:** Educational content developers requiring automated formatting and grading tools.

## Key Features (MVP)
1.  **LatexMCP Integration:** Connect to the local `latextMCP` server to compile LaTeX documents into PDFs.
2.  **Handout Generation:** Accept content topics from the teacher and generate formatted reading handouts using LaTeX.
3.  **LangGraph Orchestration:** Use LangGraph to manage the state and flow between the user and the MCP tools.
4.  **Chainlit Interface:** Provide a user-friendly chat interface for teachers to submit requests and receive generated files.

## Architecture
- **Agent Framework:** LangGraph
- **User Interface:** Chainlit
- **Tooling Protocol:** Model Context Protocol (MCP) using FastMCP
- **Infrastructure:** Local execution (Agent + MCPs on the same machine)
