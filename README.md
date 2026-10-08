# TripAI
AI-powered full-stack trip planner built with React, Node.js, Express, and MongoDB. Generates personalized itineraries using LLMs based on budget, duration, travel style, and interests, with Google Maps, weather, hotels, authentication, saved trips, and favourites.

# ✈️ TripAI — AI-Powered Trip Planner

**TripAI** is a full-stack AI-powered travel planning platform designed to help users create personalized and budget-conscious travel itineraries. The application combines **Generative AI, real-time travel APIs, maps, weather information, and accommodation/places data** to provide users with a complete trip-planning experience.

The platform allows users to enter their **starting location, destination, budget, trip duration, number of travelers, travel style, and interests**. Based on these preferences, TripAI generates a customized itinerary and provides relevant travel recommendations.


## 🚀 Key Features

### 🤖 AI-Powered Itinerary Generation
TripAI uses an **LLM-based recommendation system** to generate personalized travel itineraries based on:

- Starting location
- Destination
- Travel duration
- Number of travelers
- Budget
- Travel style
- User interests

The AI generates a structured day-by-day plan while considering the user's preferences and available budget.

### 💰 Budget-Based Trip Planning
Users can specify their approximate travel budget, allowing the application to generate recommendations that are aligned with their financial constraints.

The system can consider potential expenses such as:

- Transportation
- Accommodation
- Food
- Activities
- Attractions

### 🗺️ Interactive Maps & Location Services
The application integrates **Google Maps APIs** to provide location-based information and improve trip planning.

Planned capabilities include:

- Destination locations
- Tourist attractions
- Places of interest
- Route and distance information
- Location-based recommendations

### 🌦️ Weather Integration
Weather APIs are integrated to provide destination-specific weather information, helping users make better decisions about activities and travel plans.

Weather information can be used alongside the generated itinerary to improve the relevance of recommendations.

### 🏨 Hotels & Places Recommendations
TripAI integrates external travel and places APIs to retrieve information about:

- Hotels
- Restaurants
- Tourist attractions
- Local places
- Points of interest

This allows users to explore relevant options while planning their trip.

### 🔐 User Authentication
The application includes user authentication to provide a personalized experience.

Authenticated users can:

- Create trips
- Save trips
- Manage their travel plans
- Maintain favourite destinations/places
- Access their personalized trip information

### ❤️ Saved Trips & Favourites
Users can save generated itineraries and favourite places for future reference, allowing TripAI to function as a personal travel-planning dashboard.

### 💬 Travel Review Aggregation *(Planned)*
A future component of TripAI is a travel review aggregation system that will collect and organize reviews from multiple travel platforms to help users make better decisions.

### 👥 User-to-User Chat *(Planned)*
The project also plans to introduce a real-time communication system where users can interact with other travelers, exchange recommendations, and discuss destinations.


## 🏗️ System Architecture

TripAI follows a **full-stack architecture** consisting of a React frontend, Node.js/Express backend, MongoDB database, external APIs, and an LLM-based AI service.

                    ┌─────────────────────┐
                    │       User          │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   React Frontend   │
                    │                     │
                    │ Trip Planning UI    │
                    │ Maps & Weather      │
                    │ User Dashboard      │
                    └──────────┬──────────┘
                               │
                         REST API / HTTP
                               │
                               ▼
                    ┌─────────────────────┐
                    │ Node.js + Express   │
                    │      Backend        │
                    │                     │
                    │ Authentication      │
                    │ Trip Management     │
                    │ AI Integration      │
                    │ API Integration     │
                    └──────┬───────┬──────┘
                           │       │
                  ┌────────┘       └────────┐
                  ▼                         ▼
          ┌──────────────┐          ┌────────────────┐
          │   MongoDB    │          │ External APIs  │
          │              │          │                │
          │ Users        │          │ Google Maps    │
          │ Trips        │          │ Weather        │
          │ Favourites   │          │ Hotels/Places  │
          └──────────────┘          └────────────────┘
                                           │
                                           ▼
                                  ┌─────────────────┐
                                  │   LLM / AI      │
                                  │ Itinerary       │
                                  │ Generation      │
                                  └─────────────────┘



## 🛠️ Technology Stack

### Frontend
- **React.js**
- JavaScript
- HTML5
- CSS3
- Responsive UI design

### Backend
- **Node.js**
- **Express.js**
- REST APIs

### Database
- **MongoDB**
- MongoDB Atlas

### AI
- **Large Language Model (LLM) API**
- AI-powered itinerary generation
- Prompt-based travel recommendations

### External APIs
- **Google Maps API**
- Weather API
- Hotels / Places API

### Development Tools
- Git
- GitHub
- VS Code
- npm


## 🔄 Application Workflow

1. **User enters trip preferences**
   - Starting location
   - Destination
   - Budget
   - Number of days
   - Number of travelers
   - Travel style
   - Interests

2. **Frontend sends the request** to the backend through REST APIs.

3. **Backend processes the request** and communicates with the required external APIs.

4. **Travel data is collected**, including places, attractions, weather, maps, and accommodation information.

5. **User preferences and relevant travel information are provided to the LLM.**

6. **The AI generates a personalized itinerary** based on the user's requirements.

7. **The generated itinerary is returned to the React frontend.**

8. Users can **save the trip, manage their itinerary, and add places to favourites.**

---

## 📂 Planned Project Structure

TripAI/
│
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── hooks/
│   │   └── App.jsx
│   │
│   └── package.json
│
├── server/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── services/
│   ├── config/
│   └── server.js
│
├── README.md
├── .gitignore
└── package.json




## 🔮 Future Enhancements

The project is being developed with several additional features planned:

- 🌐 Multi-platform travel review aggregation
- 💬 Real-time user-to-user travel chat
- 🧭 Advanced route optimization
- 💰 Detailed trip expense estimation
- 📍 Personalized location recommendations
- ⭐ User reviews and ratings
- 🗺️ Interactive trip maps
- 📱 Mobile-responsive / cross-platform experience
- 🔔 Travel and weather notifications
- 🤖 Improved AI recommendations using user preferences and travel history


## 🎯 Project Objective

The primary objective of TripAI is to simplify the travel-planning process by bringing **AI-based itinerary generation, real-time travel information, maps, weather, accommodation recommendations, and personal trip management into a single platform**.

Instead of manually searching across multiple travel websites and applications, users can provide their requirements once and receive a personalized travel plan tailored to their **budget, interests, duration, and travel preferences**.



## 📌 Project Status

🚧 **Currently in Development**

Core components are being developed incrementally, including the frontend, backend, database integration, AI itinerary generation, and third-party API integrations.



## 👨‍💻 Developer

**Dhruvraj Singh Bhati**  
BCA — Vellore Institute of Technology

[GitHub](https://github.com/dhruvraj910) • [LinkedIn](https://www.linkedin.com/in/dhruvraj-singh-bhati/)
