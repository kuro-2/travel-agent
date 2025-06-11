# travel-agent
Travel Assistant is a smart chatbot built with Flask that helps users explore travel information across India. It provides real-time and fallback data for weather, train schedules, road routes, and tourist destinations, using both rule-based logic and LLM-powered intent detection.


🧳 Indian Travel Assistant (Chatbot)
This project is a smart chatbot web app that helps users explore and plan travel across India. It provides real-time and fallback data for:

🌤️ Weather conditions in major Indian cities

🚆 Train schedules (by number or between cities)

🚗 Road travel time and distance between places

🏞️ Tourist info and best time to visit Indian destinations

🔧 Features
🌐 Web-based chat UI (index.html)

🧠 Intent classification using Hugging Face LLM (with .env API key)

🗺️ Fallback support via local JSON data for offline resilience

🧩 Modular API calls for weather, trains, roads, and tourism

🚀 How to Run
Clone the repo and install dependencies
Make sure you have Python and Flask installed.

Add your Hugging Face token
Create a .env file and add:

ini
Copy
Edit
HF_TOKEN="your_huggingface_token"
Start the chat server

bash
Copy
Edit
python chat_server.py
Access in your browser
Visit http://localhost:8500

📁 Project Structure
chat_server.py – Flask app with the chat endpoint

promptflow_router.py – Intent classification and response logic

index.html – Stylish frontend for chatting

updated-*.json – Fallback data for weather, trains, roads

📌 Notes
Ensure backend APIs (/weather, /train-info, /route) are running if using live data.

Fallback JSON ensures smooth function without API access.

🧠 Sample Queries
"What's the weather in Mumbai?"

"Tell me about train 12002"

"Are there trains from Delhi to Jaipur?"

"How long to drive from Bangalore to Hyderabad?"

"Best time to visit Goa?"

