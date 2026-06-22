# 🏭 Industrial AI Assistant & RAG-Lite Analytics Platform

This project provides an AI-powered assistant and reporting dashboard that analyzes machine logs, production quantities, and downtime/failure records in manufacturing facilities to provide natural language responses. The main goal of the system is to make sense of production data, increase operational efficiency, and generate rapid insights for predictive maintenance processes.

## 🌟 Key Features

* **RAG-Lite Architecture:** Filtering data extracted from local databases (SQL/Excel) and transferring it to the LLM (Large Language Model) as a dynamic data context.
* **Semantic Routing:** A custom rule-based routing system that deterministically detects user intent and minimizes LLM hallucination.
* **Predictive Maintenance Solution Pool:** An instant recommendation engine based on root cause analysis for common industrial failures (pneumatic valves, sensor focus, motor overheating, etc.).
* **Dynamic Data Integration:** Automatically fetching live data from SQL Server and processing it on a DataFrame.
* **Modern User Interface:** A Flask-based, space-themed, animated, and interactive chat panel.

## 🛠️ Technologies Used

* **Backend:** Python, Flask, SQLAlchemy, Pandas, NumPy
* **AI & LLM:** Llama 3.1 (Localhost integration via Ollama), Custom Prompt Engineering
* **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
* **Data Sources:** MS SQL Server, Excel (`.xlsx`)

## ⚙️ Installation and Setup

You can follow the steps below to run the project locally on your machine:

### 1. Clone the Repository
```bash
git clone [https://github.com/dilaysumbul812-debug/industrial-ai-assistant.git](https://github.com/dilaysumbul812-debug/industrial-ai-assistant.git)
cd industrial-ai-assistant
2. Install Dependencies
Ensure Python is installed on your system and install the required dependencies:

Bash
pip install Flask pandas numpy sqlalchemy pyodbc requests
3. Ollama and Llama 3.1 Setup
To ensure data privacy, the project uses the Llama 3.1 model running entirely locally.

Download and install Ollama

Open your terminal, download and run the model:

Bash
ollama run llama3.1
4. Run the Application
While Ollama is running in the background, open a new terminal tab and start the Flask server:

Bash
python app.py
The application will start running at http://localhost:8080. You can interact with the assistant by navigating to this address in your browser.

📂 Project Structure
app.py: The heart of the system. Contains API routes, data manipulation, Semantic Router, and LLM communication.

uretim_tablosu.xlsx & ariza_tablosu.xlsx: Deterministic datasets analyzed by the system to base its answers on.

Raporlar/: The directory where historical PDF-based system analyses and production records are stored.

👨‍💻 Developer
Dilay Sümbül - Electrical-Electronics Engineer & AI Developer
* [LinkedIn Profilim](linkedin.com/in/dilay-sümbül-3a1961254)
* [GitHub Profilim](https://github.com/dilaysumbul812-debug)
