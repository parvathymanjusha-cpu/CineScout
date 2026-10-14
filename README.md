CineScout 🎬⚡
CineScout is a cross-platform application designed to deliver real-time weather alerts, radar updates, and automated movie schedule planning. Built with a responsive Flutter frontend and a high-performance FastAPI (Python) backend, CineScout provides users with live weather data and optimized activity tracking.

🚀 Live Web Demo: https://web-gamma-three-23.vercel.app

🌟 Key Features
Live Weather Radar & Updates: Real-time temperature, atmospheric data, and weather radar visualizations powered by OpenWeather API integration.

Smart Rescheduling: Interactive tools to reschedule and plan activities around weather forecasts.

Cross-Platform UI: Modern, responsive mobile and web interface built using Flutter.

FastAPI Backend: Lightweight RESTful API handling weather data ingestion and application services.

🛠️ Tech Stack
Frontend: Flutter / Dart (Web, Android, iOS)

Backend: Python, FastAPI, Uvicorn

APIs & Services: OpenWeather API

Deployment: Vercel (Frontend Web Hosting)

📁 Repository Structure
Plaintext
CineScout/
├── cinescout_frontend/     # Flutter application (UI, screens, widgets)
│   ├── lib/
│   │   ├── screens/        # Weather radar, rescheduling & navigation screens
│   │   └── api_service.dart
│   └── pubspec.yaml
└── CineScout- Backend/     # FastAPI Python backend server
    ├── main.py             # Server endpoints & business logic
    └── .env.example        # Environment variable templates
🚀 Getting Started Locally
Prerequisites
Flutter SDK (3.x or higher)

Python (3.9 or higher)

1. Backend Setup
Navigate to the backend directory:

Bash
cd "CineScout- Backend"
Create and activate a virtual environment (optional but recommended):

Bash
python -m venv venv
# On Windows:
.\venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
Install dependencies:

Bash
pip install fastapi uvicorn requests python-dotenv
Configure environment variables:
Create a .env file inside CineScout- Backend/ and add your OpenWeather API key:

Code snippet
OPENWEATHER_API_KEY=your_actual_api_key_here
Start the backend server:

Bash
uvicorn main:app --reload
The API will be available at http://localhost:8000.

2. Frontend Setup
Navigate to the frontend directory:

Bash
cd cinescout_frontend
Fetch dependencies:

Bash
flutter pub get
Run the app (Desktop / Browser / Emulator):

Bash
flutter run -d chrome
🔒 Security Note
Environment configuration files (.env) containing active API keys are omitted from version control for security compliance. Users running the project locally must supply their own API key in CineScout- Backend/.env.
