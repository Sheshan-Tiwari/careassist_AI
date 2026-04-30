
**CareAssist AI**

CareAssist AI is an AI-enabled healthcare assistant chatbot designed to support dementia caregivers by delivering information only from credible sources in a real-time, empathetic, and conversational manner. Built with a full-stack RAG (Retrieval-Augmented Generation) architecture, it integrates voice input/output, document-grounded responses, and a modern web interface to enhance caregiver support.


🚀 Live Demo
🔗 https://164.52.199.40:3000/


⚠️ Note: This prototype is hosted on a self-signed HTTPS server. You may need to bypass browser warnings to access it.

***

🧩 **Features**
* Conversational AI: Engages in natural language conversations, providing context-aware responses grounded in WHO dementia care documents.

* Voice Interaction: Supports voice input via Whisper ASR and voice output using Coqui TTS, facilitating hands-free communication.

* Document Retrieval: Utilizes FAISS vector search to fetch relevant information from embedded WHO PDFs.

* User-Friendly Interface: Offers a responsive and intuitive React frontend for seamless user interaction.

* Modular Architecture: Employs a microservices approach with Dockerized components for scalability and ease of deployment.

***

🏗️ **Architecture Overview**

```
.
├── app
│   ├── api
│   ├── assets
│   ├── core
│   ├── data
│   ├── main.py
│   └── services
├── data
│   ├── Dementia_World_Health_Organization.pdf
│   ├── Dementia- Information for caregivers_World_Health_Organization.pdf
│   └── Expert Q&A- Dementia and Alzheimer's Disease_World_Health_Organization.pdf
├── docker-compose.yml
├── Dockerfile
├── frontend
│   ├── Dockerfile
│   ├── index.html
│   ├── package.json
│   ├── public
│   └── src
├── models
│   └── xtts_v2_model
├── vectorstore
│   ├── index.faiss
│   └── index.pkl
└── requirements.txt
```

***

🛠️ **Tech Stack**
* Frontend: React, Tailwind CSS, Vite

* Backend: FastAPI, LangChain, FAISS

* Audio Processing: Whisper (ASR), Coqui TTS

* Containerization: Docker, Docker Compose

* Deployment: Self-hosted on a cloud VM (IPv4: 164.52.199.40)

***

🧪 **Testing the Application**
* Voice Input: Click on the microphone icon to speak your query.

* Text Input: Type your question in the input box and press Enter.

* Voice Output: Responses will be read aloud using Coqui TTS.

***

📁 **Data Sources**

* The chatbot retrieves information from the following WHO documents:

    * Dementia: A Public Health Priority

    * Dementia: Information for Caregivers

    * Expert Q&A: Dementia and Alzheimer's Disease

* These documents are embedded into a FAISS vector store for efficient retrieval.

***

🧠 **Future Enhancements**

* Multilingual Support: Extend capabilities to support multiple languages.

* Large credible data source for RAG

* Mobile Responsiveness: Optimize the frontend for mobile devices.

* Analytics Dashboard: Provide insights into user interactions and common queries.
