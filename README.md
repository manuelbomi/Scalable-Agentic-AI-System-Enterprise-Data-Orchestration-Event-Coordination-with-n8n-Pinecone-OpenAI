# Scalable Agentic AI System: Enterprise Data Orchestration & Event Coordination with n8n, Pinecone & OpenAI

### Overview  

#### This repository contains a multifunctional Agentic AI workflow built in n8n. The system leverages OpenAI, Pinecone, and Google Calendar to provide enterprise-ready orchestration across two core functions:
    1. Enterprise Data Orchestration
    
        ◦ Store and retrieve documents from enterprise repositories (e.g., Google Drive) using Pinecone vector storage.
        
        ◦ Generate OpenAI embeddings for semantic search, knowledge retrieval, and intelligent querying.
        
    2. Event Coordination
        ◦ Automate scheduling by checking availability in Google Calendar.
        
        ◦ Create events in confirmed time slots, acting as a smart AI-powered calendar assistant.
        
#### This workflow demonstrates how Agentic AI can serve as the foundation for enterprise automation, combining data management and business operations into a single extensible architecture.

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

  

### System Architecture    
The workflow integrates multiple components inside n8n:
    • Chat Input → Handles user queries and starts AI-agentic interactions.
    
    • OpenAI Chat Model (GPT-4o-mini) 🠊 Provides natural language reasoning and conversational orchestration.
    
    • Simple Memory 🠊 Maintains short-term conversational state.
    
    • Google Calendar Tools 🠊
        ◦ Get Availability: Finds open time slots.
        
        ◦ Create Events: Books events once confirmed.
        
    • Pinecone Vector Store 🠊 Stores and retrieves vectorized enterprise documents for semantic search.
    
    • OpenAI Embeddings 🠊 Generates embeddings that power Pinecone search and retrieval.


### How to Integrate the Project Into Your Enterprise Workflow  

#### 1. Clone the Repository
git clone https://github.com/manuelbomi/Scalable-Agentic-AI-System-Enterprise-Data-Orchestration-Event-Coordination-with-n8n-Pinecone-OpenAI
cd <your-repo-name>

#### 2. Import into n8n
     
   * Open your local or hosted n8n instance.
       
   * Go to Workflows 🠊 Import from File.
       
   * Upload Multi_fucntional_Agentic_AI.json.
       
#### 3. Configure Credentials

The workflow requires valid API keys and credentials:

    • OpenAI API Key 🠊 for chat and embeddings.
   
    • Pinecone API Key 🠊 for vector storage.
   
    • Google Calendar OAuth 🠊 for event scheduling and availability lookup.
   
* Set these up under n8n 🠊 Credentials.

####  5. Run the Workflow

    • Activate the workflow.
   
    • Open the chat interface.
   
    • Start interacting with the AI agent.


### Example Use Cases for Enterprise Workflows  

    • Enterprise Data Management 🠊 Upload and retrieve business documents, knowledge bases, or policies from Pinecone.
    
    • Calendar Assistant 🠊 Schedule client meetings, team syncs, or enterprise events automatically.
    
    • Knowledge Querying 🠊 Ask questions against stored enterprise repositories.
    
    • Multimodal Extensions (Future) 🠊 Integrate with email, Slack, Teams, or CRMs for broader enterprise adoption.
    
---

### How the Agent was Designed   

#### If you decide to use n8n to design the Agent in a step-by-step fashion as opposed to cloning this repository, then do the following:

####  Start with this workflow here: https://github.com/manuelbomi/Enterprise-Agentic-AI---Scalable-Meeting-Orchestration-with-n8n
  
<img width="1366" height="768" alt="1 start with this workflow" src="https://github.com/user-attachments/assets/2e9fc90d-7c7e-48e2-ac2e-8a0ac6fb6713" />

---

#### After completing the starter workflow, then look for vector store tool
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/a408d849-9cd0-4da8-9075-c6156378df95" />

#### Tool description

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/0bd47825-0755-4b12-b624-5c97b9712d2c" />

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/84d9f262-1be1-44f2-9c91-ce2191a3c984" />

---

#### Select Pinecone Namespace

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/7354a6f2-1360-41cd-ac6d-0bc1a5821e7c" />

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/43e5ca44-3060-412c-947b-43b25c0d2d3a" />

---

#### Click on embeddings and select embeddings open ai

<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/378e2921-f363-4174-be5b-fc8f3248cb42" />

---

#### Select the test embeddings 3 small
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/3e86cbb9-8959-40a9-a00c-70e7f0b0b1ac" />

---

#### Start using the Agent to answer questions and schedule meetings:
<img width="1366" height="768" alt="Image" src="https://github.com/user-attachments/assets/4562fa07-24a5-400b-aca2-48b242d81686" />

---



### Scalability & Extensions for Additional Enterprise Workflows 🔧 

#### This system is designed to scale into multi-domain enterprise AI orchestration:

    • Additional Enterprise Data Sources 🠊 Connect Google Drive, Notion, Confluence, or internal databases.
    
    • More Vector Databases 🠊 Swap Pinecone with alternatives like Weaviate, Milvus, or ChromaDB.
    
    • Event Coordination Extensions 🠊 Integrate with Outlook, Teams, or Zoom APIs.
    
    • Advanced Agentic Patterns 🠊 Chain multiple AI agents for specialized tasks (e.g., finance, HR, compliance).
    
    • Deployment Options 🠊
    
        ◦ Run in Dockerized n8n for enterprise DevOps.
        
        ◦ Deploy behind enterprise SSO & security gateways.
        
        ◦ Integrate with Kubernetes clusters for high availability.

---

### How to Deploy in Enterprise Settings  :

#### For enterprise use, this workflow can be:

    • Dockerized and deployed in cloud platforms (AWS, GCP, Azure).
    
    • Secured with API gateways and role-based access control.
    
    • Integrated into existing IT workflows (e.g., HR systems, CRMs, ERP).
    
    • Monitored with observability tools for scaling and reliability.

---
    
License
This project is released under the MIT License.


Thank you for reading 

---


### **AUTHOR'S BACKGROUND**
### Author's Name:  Emmanuel Oyekanlu
```
Skillset:   I have experience spanning several years in data science, developing scalable enterprise data pipelines,
enterprise solution architecture, architecting enterprise systems data and AI applications,
software and AI solution design and deployments, data engineering, high performance computing (GPU, CUDA), machine learning,
NLP, Agentic-AI and LLM applications as well as deploying scalable solutions (apps) on-prem and in the cloud.

I can be reached through: manuelbomi@yahoo.com

Websites (professional):  http://emmanueloyekanlu.com/
Websites (application):  https://app.emmanueloyekanluprojects.com/
Publications:  https://scholar.google.com/citations?user=S-jTMfkAAAAJ&hl=en
LinkedIn:  https://www.linkedin.com/in/emmanuel-oyekanlu-6ba98616
Github:  https://github.com/manuelbomi

```
[![Icons](https://skillicons.dev/icons?i=aws,azure,gcp,scala,mongodb,redis,cassandra,kafka,anaconda,matlab,nodejs,django,py,c,anaconda,git,github,mysql,docker,kubernetes&theme=dark)](https://skillicons.dev)



