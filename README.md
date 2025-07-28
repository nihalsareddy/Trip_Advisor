Absolutely! Here's your updated, **clean README** for the **Trip Advisor AI project**, this time with **OpenAI** (instead of Ollama) as the LLM provider:

---

# ✈️ Trip Advisor – AI-Powered Travel Planner

**Trip Advisor** is an AI-powered web application that generates detailed, personalized travel itineraries based on your destination, dates, and interests. It uses **OpenAI’s language models** along with **CrewAI** and **LangChain** to orchestrate a team of intelligent agents that collaboratively research, plan, and deliver complete day-by-day travel guides.

---

## 🚀 Features

* **🧭 Personalized Itineraries** – Plans tailored to your travel preferences (e.g., adventure, food, culture).
* **📍 Comprehensive Travel Plans** – Includes:

  * 🎡 Sightseeing recommendations
  * 🍽️ Local cuisine suggestions
  * 🏨 Accommodation ideas & budget guidance
  * 🚆 Transportation tips and visa info
* **🤖 AI Agent Collaboration** – Uses a CrewAI-based multi-agent system.
* **🌐 Simple Web Interface** – Built with Streamlit for easy input and output.
* **📥 Exportable Results** – Download your complete itinerary as a `.txt` file.

---

## ⚙️ How It Works

The system uses **CrewAI** to orchestrate a multi-agent workflow:

| 🧠 Agent             | 🛠️ Role                                                   |
| -------------------- | ---------------------------------------------------------- |
| **Location Expert**  | Collects key data on visas, weather, cost, and transport   |
| **City Local Guide** | Suggests top attractions, food spots, and local events     |
| **Travel Planner**   | Compiles everything into a coherent day-by-day travel plan |

These agents communicate using **LangChain** and generate responses via **OpenAI’s GPT models**. Web search tools (via DuckDuckGo) enhance real-time accuracy.

---

## 🛠️ Technologies Used

* **Backend:** Python
* **AI Framework:** CrewAI
* **LLM Integration:** OpenAI API + LangChain
* **Frontend:** Streamlit
* **Web Search Tool:** DuckDuckGo Search

---

## 🗂️ Project Structure

```
Trip_Advisor/
├── app.py              # Streamlit app
├── Travel_agents.py    # CrewAI agent setup
├── Travel_Tasks.py     # Defines tasks per agent
├── Travels_tools.py    # Tools for data gathering (e.g., search)
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation
```

---

## 🧪 Setup & Installation

### Prerequisites

* Python 3.8 or higher
* OpenAI API key (get one from [https://platform.openai.com](https://platform.openai.com))

---

### Steps to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/Trip_Advisor.git
cd Trip_Advisor

# 2. Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Set your OpenAI API Key
export OPENAI_API_KEY=your-key-here  # On Windows: set OPENAI_API_KEY=your-key-here

# 5. Launch the app
streamlit run app.py
```

Then open your browser at: [http://localhost:8501](http://localhost:8501)

---

## ▶️ How to Use

1. **Enter Trip Details**

   * From City
   * Destination
   * Travel Dates
   * Interests (e.g., “nature, local food, museums”)

2. **Click “🚀 Generate Travel Plan”**
   Watch agents collaborate to build your plan.

3. **Review & Download**
   Your full itinerary appears on-screen and can be downloaded as a `.txt` file.

---

## 🤝 Contributing

Contributions are welcome!

```bash
# Fork → Branch → Commit → Push → Pull Request
git checkout -b feature/your-feature
git commit -m "Add new feature"
git push origin feature/your-feature
```

---

## 📄 License

This project is licensed under the **MIT License**.

---

Let me know if you want a demo section with screenshots or video, or instructions to deploy this to **Render**, **Replit**, or **Streamlit Cloud**.
