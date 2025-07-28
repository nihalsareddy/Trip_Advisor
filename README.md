Trip Advisor ✈️
Welcome to Trip Advisor, an AI-powered travel planner designed to create personalized and detailed itineraries for your next adventure. By leveraging the power of AI agents from crewai, this application takes your destination, dates, and interests to generate a comprehensive travel plan, including sightseeing, dining, accommodation, and transportation logistics.

✨ Features
Personalized Itineraries: Get travel plans tailored to your specific interests, whether you're a foodie, an adventurer, or a history buff.

Comprehensive Details: The generated plan includes everything you need:

🎡 Attractions and activities

🍕 Local food recommendations

🏨 Accommodation suggestions and budget planning

🚆 Transportation details and visa information

AI-Powered Agents: A crew of specialized AI agents collaborates to gather, analyze, and structure the perfect trip for you.

User-Friendly Interface: A simple web interface built with Streamlit makes it easy to input your travel details and receive your plan.

Downloadable Plans: Save your generated travel plan as a text file for offline access.

⚙️ How It Works
This project uses the crewai framework to orchestrate a team of autonomous AI agents. Each agent has a specific role and works sequentially to build the final travel plan.

Location Expert: This agent gathers essential logistical information about the destination, such as weather, transportation options, cost of living, and visa requirements.

City Local Guide Expert: This agent acts as a local guide, finding the best attractions, restaurants, and events based on your stated interests.

Travel Planning Expert: This agent takes all the information gathered by the other two agents and compiles it into a structured, day-by-day itinerary, complete with a city introduction and helpful tips.

The application is powered by a local Large Language Model (LLM) via Ollama (llama3.2) and uses DuckDuckGo for real-time web searches to ensure the information is up-to-date.

🛠️ Technologies Used
Backend: Python

AI Framework: CrewAI

LLM Integration: LangChain, Ollama

Web Interface: Streamlit

Web Search: DuckDuckGo Search

🚀 Setup and Installation
Follow these steps to get the Trip Advisor application running on your local machine.

Prerequisites
Python 3.8 or higher

Ollama installed and running.

The llama3.2 model pulled in Ollama. You can get it by running:

ollama pull llama3.2

Installation Steps
Clone the Repository

git clone https://github.com/your-username/Trip_Advisor.git
cd Trip_Advisor

Create a Virtual Environment
It's recommended to create a virtual environment to manage project dependencies.

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

Install Dependencies
Install all the required Python packages using the requirements.txt file.

pip install -r requirements.txt

▶️ How to Use
Run the Streamlit App
Make sure your Ollama server is running in the background. Then, start the Streamlit application:

streamlit run app.py

Open in Browser
Your web browser should automatically open to the application's URL (usually http://localhost:8501).

Fill in Your Trip Details

From City: The city you'll be traveling from.

Destination City: Where you want to go.

Departure Date: The start date of your trip.

Return Date: The end date of your trip.

Your Interests: A description of what you enjoy (e.g., "historical sites, hiking, and trying local coffee shops").

Generate Your Plan
Click the "🚀 Generate Travel Plan" button. The AI agents will start their work. You can see their progress in the terminal where you launched Streamlit.

View and Download
Once complete, the full travel itinerary will be displayed on the page. You can read it there or click the "📥 Download Travel Plan" button to save it as a .txt file.

📂 Project Structure
Trip_Advisor/
├── app.py              # The main Streamlit application file
├── Travel_agents.py    # Defines the CrewAI agents (Location, Guide, Planner)
├── Travel_Tasks.py     # Defines the tasks for each agent
├── Travels_tools.py    # Defines the tools used by agents (e.g., web search)
├── requirements.txt    # Lists the Python dependencies for the project
└── README.md           # This file

🤝 Contributing
Contributions are welcome! If you have ideas for new features or improvements, feel free to fork the repository, make your changes, and submit a pull request.

Fork the repository.

Create a new branch (git checkout -b feature/your-feature-name).

Commit your changes (git commit -m 'Add some amazing feature').

Push to the branch (git push origin feature/your-feature-name).

Open a Pull Request.

📄 License
This project is open-source and available under the MIT License.
