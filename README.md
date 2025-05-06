# ai_challenge
HR AI Agent for Startup Hiring
This project is an agentic AI application designed to help HR professionals plan the hiring process for early-stage startups. Built with Langflow, GPT-4o, and integrated tools like Google Search, the agent can perform multi-step reasoning, generate job descriptions, suggest checklists, and maintain memory throughout the conversation.
Features:-
🧠 Conversational Agent: Interactively asks clarifying questions (budget, timeline, roles).

📝 Job Description Generator: Creates tailored JD drafts.

✅ Hiring Checklist Builder: Outputs a structured, actionable hiring plan.

🌐 Tool Use: Integrates Google Search API to gather real-world data (e.g. salary benchmarks).

💾 Memory Retention: Maintains conversation context for multi-turn interaction.

🧰 Tech Stack used:-
| Layer               | Technology                | Purpose                                        |
| ------------------- | ------------------------- | ---------------------------------------------- |
| **LLM**             | OpenAI GPT-4o             | Powers the conversational agent                |
| **Agent Framework** | Langflow                  | Visual orchestration of agent, tools, and flow |
| **Search Tool**     | Google Search API         | Augments answers with real-time web data       |
| **Frontend**        | Jupyter Notebook / Python | Interactive test environment for agent         |
| **Backend**         | REST API via Langflow     | Executes agent flow hosted on Astra DB infra   |

🧠 Design Decisions:-
Langflow for Orchestration
Langflow’s visual interface makes it easy to connect tools, define memory, and manage multi-step flows.

Tool Integration
Google Search API enables the agent to validate assumptions (e.g., role responsibilities, salary benchmarks).

Memory Management
Full conversation history is appended to each user query and preserved during the session.

Jupyter Interface
Used for rapid prototyping and showcasing conversational flow with formatted markdown outputs.

Markdown Output
Agent responses are rendered cleanly for both humans and potential system parsing

📌 Architecture:-

User input is captured through a notebook or interface.

Langflow routes queries to the OpenAI model and tools.

Google Search API is called when additional info is needed.

Output is structured as markdown/JSON and rendered back.

🛠 Improvements (With More Time):-
| Area                 | Suggestion                                              |
| -------------------- | ------------------------------------------------------- |
| **Security**         | Store API keys in `.env` and use `dotenv` to load them. |
| **Web Interface**    | Add a Streamlit or Flask-based frontend.                |
| **Checklist Export** | Allow output as downloadable PDFs or JSON.              |
| **Tool Expansion**   | Add resume screening, email drafting tools.             |
| **Persistence**      | Store chat logs in a database or session file.          |


Below is the architecture diagram which i have used to develop this application 



