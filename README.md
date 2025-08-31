# Campus Connect 🚀

**College Events Aggregator**  
A modern events aggregator that collects hackathons, internships, and placement opportunities from multiple platforms into one clean interface. Students can sign in with Gmail and get personalized notifications.

---

## 🛠️ Tech Stack

- **Frontend:** React 18 + TypeScript + Tailwind CSS  
- **Backend:** Node.js + Express + TypeScript  
- **Database:** MongoDB Atlas (Free tier)  
- **Authentication:** Google OAuth 2.0  
- **Web Scraping:** Puppeteer + Cheerio  
- **Notifications:** Real-time updates with Socket.io  
- **Deployment:** Vercel (Frontend) + Railway (Backend) - Both free  

---

## 🗄️ Database Setup (MongoDB Atlas)

- Go to MongoDB Atlas and create a free account
- Create a new cluster (M0 Sandbox - Free)
- Create a database user
- Whitelist IP addresses (0.0.0.0/0 for development)
- Get connection string and add it to .env

## 🔑 Google OAuth Setup

- Go to Google Cloud Console
- Create a new project or select an existing one
- Enable Google+ API
- Create OAuth 2.0 credentials
- Add authorized origins:
  http://localhost:3000
- Add authorized redirect URIs:
  http://localhost:3000/auth/callback
- Copy Client ID and Client Secret to your .env files

## 🔧 Implementation Files
- Backend Implementation
Authentication: Google OAuth integration
Web Scrapers: For Unstop, HackerEarth, Internshala
Real-time Updates: Socket.io for live notifications
Database Models: User, Event, Notification schemas
API Routes: RESTful endpoints for all operations
Cron Jobs: Automated scraping every hour

- Frontend Implementation
Modern UI: Clean design with Tailwind CSS
Real-time Updates: Live event notifications
Filtering: By category, date, location
Bookmarking: Save interesting events
Responsive Design: Mobile-friendly interface

## ⭐ Key Features
User Features
Google Authentication: Secure login with Gmail
Event Dashboard: Centralized view of all opportunities
Smart Filtering: Filter by type, date, skills required
Bookmarks: Save events for later

## 🚀 Running the Project
- Backend
cd backend
npm install
npm run dev

- Frontend
cd frontend
npm install
npm start

