
---

# ✈️ Trip Advisor – AI-Powered Travel Planner

**Trip Advisor** is an AI-powered application that generates detailed, personalized travel itineraries based on your preferences, dates, and destination. Built with **Python**, **CrewAI**, and **LangChain**, it orchestrates a team of AI agents that collaborate to research logistics, recommend attractions and food, and plan your trip day-by-day.

---

## 🚀 Features

* **🧭 Personalized Itineraries** – Get custom plans based on your travel style (foodie, adventurer, history buff, etc.).
* **📍 Comprehensive Details** – Suggestions for:

  * 🌆 Attractions & activities
  * 🍜 Local food
  * 🏨 Accommodation & budgeting
  * 🚆 Transportation & visa logistics
* **🤖 Multi-Agent System** – Uses CrewAI to coordinate specialized AI agents.
* **🌐 Streamlit UI** – Simple interface to enter trip info and generate plans.
* **📥 Download Option** – Save your itinerary as a text file for offline use.

---

## ⚙️ How It Works

This project uses **CrewAI** to coordinate a team of AI agents:

| Agent                | Role                                                      |
| -------------------- | --------------------------------------------------------- |
| **Location Expert**  | Gathers visa, weather, cost-of-living, and transit data   |
| **City Local Guide** | Finds local attractions, restaurants, and events          |
| **Travel Planner**   | Combines everything into a structured itinerary with tips |

Agents are powered by **LangChain** and **Ollama’s Llama3.2 LLM**, using **DuckDuckGo** for real-time data.

---

## 🛠️ Technologies Used

* **Backend:** Python
* **AI Orchestration:** CrewAI
* **LLM Integration:** LangChain + Ollama (Llama3.2)
* **Web Interface:** Streamlit
* **Web Search:** DuckDuckGo Search

---

## 🗂️ Project Structure

```
Trip_Advisor/
├── app.py              # Streamlit main app
├── Travel_agents.py    # Defines CrewAI agents
├── Travel_Tasks.py     # Task definitions for each agent
├── Travels_tools.py    # Tool functions (e.g., DuckDuckGo search)
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

---

## 🧪 Setup & Installation

### Prerequisites

* Python 3.8+
* OpenAI
* Ollama installed and running
  Get Llama3.2 model:

  ```
  ollama pull llama3:2
  ```

### Steps

```bash
# 1. Clone the repo
git clone https://github.com/your-username/Trip_Advisor.git
cd Trip_Advisor

# 2. Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the app
streamlit run app.py
```

Then go to: [http://localhost:8501](http://localhost:8501)

---

## ▶️ How to Use

1. **Fill your trip details:**

   * From City
   * Destination City
   * Travel Dates
   * Interests (e.g., “food, hiking, history”)

2. **Click “🚀 Generate Travel Plan”**
   The agents will begin working—status shown in terminal.

3. **View & Download**
   See your full itinerary and download it as `.txt`.

---

## 🤝 Contributing

Pull requests are welcome!

1. Fork the repo
2. Create a branch: `git checkout -b feature/your-feature`
3. Commit changes: `git commit -m "Add feature"`
4. Push: `git push origin feature/your-feature`
5. Submit a Pull Request

---

## 📄 License

This project is open-sourced under the **MIT License**.

---

Let me know if you want a matching **badge header**, **demo video embed**, or **live deployment link section** added!
