## Day 11 of 15-day challenge

# Nutriagent

# 🧠 AI-Powered Diet Guide

An intelligent wellness assistant that helps users set personal health goals—such as building muscle, achieving glowing skin, aging healthily, or managing health conditions—and get customized diet plans using AI. The future scope includes **agentic AI** that can **place supplement or grocery orders** based on personalized nutrition needs.

---

## ✅ Current Status

🟢 **Frontend: Completed**  
🔴 **Backend & Database: In Progress / Planned**

---

## 📸 Features (Frontend)

- 🧾 Wellness goal selection interface
- 🧍‍♂️ Onboarding and profile setup screens
- ⚡ Fast, responsive, modern UI using React.js + Tailwind CSS
- 🔀 Route-based navigation for Home, Profile, Goals, Suggestions
- ✨ Clean layout for future integration with personalized meal plans and order actions

---

## 🧱 Tech Stack

### 🔹 Frontend
- **Framework:** React.js
- **Styling:** Tailwind CSS
- **Routing:** React Router

### 🔹 Backend *(Planned)*
- **Framework:** Node.js + Express.js
- **AI Microservice:** Python (FastAPI or Flask) for dietary suggestion logic and LLM integration
- **Agentic Layer:** LangChain Agents + OpenAI Function Calling or custom Python-based agent flow
- **Order Handling:** Integration with APIs (Instacart, Amazon, or mock ordering service)

### 🔹 Database *(Planned)*
- **MongoDB:** For user profiles, goals, and generated plans
- **(Optional)** Redis: For caching frequently used plans

### 🔹 Other Tools
- **Authentication:** Firebase Auth or JWT
- **APIs:** Nutritionix / Spoonacular (for food and nutrition data)
- **Cloud:** 
  - Frontend: Vercel or Netlify  
  - Backend: Render, Railway, or AWS  
  - Python AI Service: Railway, Heroku, or EC2 Dockerized
- **Media Storage:** Firebase Storage or Cloudinary (for user-uploaded images)

---

## 🗂️ Step-by-Step Development Planner

### ✅ Phase 1: Project Setup (Frontend Done ✅, Backend Planned 🔜)

**Frontend (✅ Done):**
- Initialize React project
- Set up Tailwind CSS
- Set up routing (Home, Profile, Goals, Suggestions)
- UI for onboarding, goal selection, user profile

**Backend (🔜 Planned):**
- Initialize Node.js + Express.js backend
- Connect MongoDB using Mongoose
- Build basic REST API structure

---

### ✅ Phase 2: User Flow & Goal Setting *(Planned)*

**Frontend (✅ Done):**
- Create user onboarding and goal selection forms
- Design responsive forms for wellness categories

**Backend (🔜 Planned):**
- `POST /user` – Create user
- `PUT /goals` – Set/update wellness goals
- `GET /profile` – Fetch user data
- Store all data in MongoDB

---

### ✅ Phase 3: Diet Suggestion Engine (AI Core) *(Planned)*

**Tasks:**
- Create Python microservice using FastAPI or Flask
- Accept user profile + goal input → Output JSON meal plan
- Use OpenAI or another LLM for generating personalized diets
- Incorporate prompt engineering & health-based reasoning

**Example Prompt:**
> "Generate a 3-day meal plan for a 25-year-old female aiming for glowing skin. Avoid dairy and gluten. Focus on high antioxidants."

**Integration:**
- Node.js backend calls the Python service
- Store results per user in MongoDB

---

### ✅ Phase 4: Agentic AI for Action-taking *(Planned)*

**Tasks:**
- Define agent actions like:
  - “Place grocery order”
  - “Suggest supplements”
  - “Add meals to calendar”
- Build LangChain Agent with OpenAI + HTTP tool
- Use Function Calling to simulate order placements
- Start with dummy API integrations, scale to real APIs (Amazon, iHerb, Instacart)

---

### ✅ Phase 5: User Dashboard & Feedback Loop *(Planned)*

**Frontend Tasks:**
- Display personalized meal plan UI
- Buttons for grocery/supplement orders
- Feedback: “Was this helpful?”, “Suggest alternatives”

**Backend Tasks:**
- Track user clicks, feedback
- Analyze usage data to refine recommendations

---

### ✅ Phase 6: Polishing & Extras *(Planned)*

- 🔐 **Authentication:** Firebase Auth or JWT to protect user data
- 📣 **Notifications:** Email or push notifications for meal reminders, order updates
- 📊 **Analytics:** Show user progress, plan effectiveness, and streaks
- ☁️ **Deployment:**
  - Frontend → Vercel or Netlify
  - Backend → Render or Railway
  - Python AI Service → Railway / Heroku / Dockerized EC2

---

## 📦 Bonus Features (Future Ideas)

- ✨ Daily wellness tips powered by LLMs
- 🎙️ Voice input to set goals or request recommendations
- 💬 AI Chatbot interface for dietary Q&A

---

## 🛠️ How to Run the Frontend Locally

---

## 📌 How to Contribute

1. Fork the repo
2. Create a new branch (`git checkout -b feature-branch`)
3. Make your changes and commit
4. Push to the branch (`git push origin feature-branch`)
5. Create a pull request

---

## 📄 License

MIT License – feel free to use and modify!

```bash
git clone https://github.com/vedant2402/ai-powered-diet-guide.git
cd ai-powered-diet-guide
npm install
npm run dev
