# Project--Ascend
Project Ascend 🚀
https://drive.google.com/drive/folders/1PrEpmYnfB8b5FM7AUr50vpomf7sc0F65?usp=sharing
Project Ascend is an AI-powered personalized learning and productivity ecosystem. It combines an Agentic RAG (Retrieval-Augmented Generation) tutor, a dynamic task planner, and a vision-based integrity monitor to help students stay on track with their educational "quests".
+4

🌟 Key Features

Nexus AI Tutor (Online & Offline): A smart tutor that searches your local knowledge base (PDFs) to answer questions.
+1


Online Mode: Uses GPT-3.5 Turbo for advanced reasoning and web search via Tavily.
+1


Offline Mode: Powered by a local Phi-3 Mini model for privacy and offline access.

AI Quest Planner: Set a "Main Quest" and a duration. The system uses AI to generate a day-by-day roadmap with practical tasks.
+2


Integrity Monitor: A computer vision tool that uses facial landmark detection to ensure you stay focused during study sessions, alerting you if you turn away or leave the screen.

Progress Tracking & Gamification: Earn EXP points for completing tasks. Track your weekly consistency with generated charts and progress summaries.
+3


Automated Resource Recommender: Automatically finds relevant YouTube tutorials and documentation (from sites like GeeksforGeeks) based on your queries.

🛠️ Technical Stack

Language: Python 3.13 
+1


AI Frameworks: LangChain, LangGraph, OpenAI GPT-3.5/4o, Llama-cpp 
+3


Vector Database: ChromaDB (for PDF ingestion and retrieval) 


Web Framework: FastAPI 
+1


Computer Vision: OpenCV, Dlib (for facial tracking) 
+1


Database: SQLite (for task and EXP management) 

🚀 Getting Started
1. Installation
Clone the repository and install the dependencies:

Bash

pip install -r requirements.txt
2. Configuration

Environment Variables: Set your OPENAI_API_KEY and TAVILY_API_KEY in the environment or directly in the configuration files (e.g., main_api.py, ask_tutor.py).
+2


Facial Landmark Model: Ensure shape_predictor_68_face_landmarks.dat is in the root directory for the Integrity Monitor.

3. Usage

Ingest Documents: Place PDFs in the knowledge_base folder and run python ingest_data.py to populate the AI's memory.


Start the AI Agent: Run python ask_tutor.py to chat with your tutor.


Launch the API: Run python main_api.py to start the backend server for task management and progress tracking.
+1


Monitor Focus: Run python integrity_monitor.py to start the webcam focus tracker.

📂 Project Structure

ask_tutor.py: The main chat interface for Nexus AI.


main_api.py: FastAPI backend for the quest and EXP system.
+1


integrity_monitor.py: Focus tracking using computer vision.


ingest_data.py: Script to process and vectorize PDF knowledge.


recommender.py: Tools for YouTube and web documentation search.


database_setup.py: Initializes the SQLite schema for users and quests.


Created as part of the Project Ascend development suite.
