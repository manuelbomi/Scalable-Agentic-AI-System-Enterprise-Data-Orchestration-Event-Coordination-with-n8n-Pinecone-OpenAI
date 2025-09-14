# Scalable Agentic AI System: Enterprise Data Orchestration & Event Coordination with n8n, Pinecone & OpenAI

Overview 📌 
This repository contains a multifunctional Agentic AI workflow built in n8n. The system leverages OpenAI, Pinecone, and Google Calendar to provide enterprise-ready orchestration across two core functions:
    1. Enterprise Data Orchestration
        ◦ Store and retrieve documents from enterprise repositories (e.g., Google Drive) using Pinecone vector storage.
        ◦ Generate OpenAI embeddings for semantic search, knowledge retrieval, and intelligent querying.
    2. Event Coordination
        ◦ Automate scheduling by checking availability in Google Calendar.
        ◦ Create events in confirmed time slots, acting as a smart AI-powered calendar assistant.
This workflow demonstrates how Agentic AI can serve as the foundation for enterprise automation, combining data management and business operations into a single extensible architecture.

---

### Agent's Components

    • n8n for workflow automation.
    • OpenAI for conversational reasoning & embeddings.
    • Pinecone for vector storage.
    • Google Calendar API for scheduling integration.

---
### The Agent 

* The AI Agent has the autonomy to select any component that it wants to do any of its work

<img width="997" height="433" alt="Image" src="https://github.com/user-attachments/assets/2330fb6f-7fe4-48fd-98e9-1806b073e139" />
---

### The Agent Can Multi-task: 
  * (1) Can Orchestrate Enterprise Data Between an Enterprise Repository and a Vector Database (Pinecone).
    
    ##### It can then use the data in the vector database to answer enterprise related questions.

    <img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/2baebcec-bc1b-4226-888f-ffd336fcee4f" />
    
    <img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/15ee2fdb-b525-4042-ae6f-7c5d37e9350f" />

    <img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/7302cd0a-d6d6-4131-95bf-fb3cf683c13f" />

---

  * (2) Can Coordinate Events Such As Scheduling Meetings
    <img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/fb5a2144-8bfb-4d53-acdb-1f69c3124d73" />
    
  <img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/60b169b0-bcc8-4c6a-82b9-69ceca1e55f0" />
  
  <img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/b8d6f0cb-f411-4250-a74f-4ed53889af06" />
  
  <img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/af92200a-991e-410e-af9c-7edb771cc2ab" />

  



⚙️ System Architecture
The workflow integrates multiple components inside n8n:
    • Chat Input → Handles user queries and starts AI-agentic interactions.
    • OpenAI Chat Model (GPT-4o-mini) → Provides natural language reasoning and conversational orchestration.
    • Simple Memory → Maintains short-term conversational state.
    • Google Calendar Tools →
        ◦ Get Availability: Finds open time slots.
        ◦ Create Events: Books events once confirmed.
    • Pinecone Vector Store → Stores and retrieves vectorized enterprise documents for semantic search.
    • OpenAI Embeddings → Generates embeddings that power Pinecone search and retrieval.


📂 Repository Contents
    • Multi_fucntional_Agentic_AI.json → The exported n8n workflow file.

🚀 Getting Started
1. Clone the Repository
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>



2. Import into n8n
    1. Open your local or hosted n8n instance.
    2. Go to Workflows → Import from File.
    3. Upload Multi_fucntional_Agentic_AI.json.
3. Configure Credentials
The workflow requires valid API keys and credentials:
    • OpenAI API Key → for chat and embeddings.
    • Pinecone API Key → for vector storage.
    • Google Calendar OAuth → for event scheduling and availability lookup.
Set these up under n8n → Credentials.
4. Run the Workflow
    • Activate the workflow.
    • Open the chat interface.
    • Start interacting with the AI agent.


💡 Example Use Cases
    • Enterprise Data Management → Upload and retrieve business documents, knowledge bases, or policies from Pinecone.
    • Calendar Assistant → Schedule client meetings, team syncs, or enterprise events automatically.
    • Knowledge Querying → Ask questions against stored enterprise repositories.
    • Multimodal Extensions (Future) → Integrate with email, Slack, Teams, or CRMs for broader enterprise adoption.
    
---

### How the Agent was Designed  💡 

* Start with this workflow:
  Details regarding how to design the workflow could be obtained here: 
<img width="1366" height="768" alt="1 start with this workflow" src="https://github.com/user-attachments/assets/2e9fc90d-7c7e-48e2-ac2e-8a0ac6fb6713" />


🔧 Scalability & Extensions
This system is designed to scale into multi-domain enterprise AI orchestration:
    • Additional Enterprise Data Sources → Connect Google Drive, Notion, Confluence, or internal databases.
    • More Vector Databases → Swap Pinecone with alternatives like Weaviate, Milvus, or ChromaDB.
    • Event Coordination Extensions → Integrate with Outlook, Teams, or Zoom APIs.
    • Advanced Agentic Patterns → Chain multiple AI agents for specialized tasks (e.g., finance, HR, compliance).
    • Deployment Options →
        ◦ Run in Dockerized n8n for enterprise DevOps.
        ◦ Deploy behind enterprise SSO & security gateways.
        ◦ Integrate with Kubernetes clusters for high availability.

🏢 Enterprise Deployment
For enterprise use, this workflow can be:
    • Dockerized and deployed in cloud platforms (AWS, GCP, Azure).
    • Secured with API gateways and role-based access control.
    • Integrated into existing IT workflows (e.g., HR systems, CRMs, ERP).
    • Monitored with observability tools for scaling and reliability.
📜 License
This project is released under the MIT License.

⭐ 
