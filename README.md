# 🌿 Green Intelligence: AI for a Sustainable Planet

**Tagline:** "Code that saves carbon."

A full-stack AI-powered sustainability dashboard that helps users track their Energy, Water, and Carbon usage, view personalized analytics, and receive AI-generated recommendations to reduce their environmental footprint.

## 🚀 Features

- **User Authentication** - Firebase Authentication with email/password login and signup
- **Forgot Password** - OTP-based password reset simulation
- **Consumption Tracking** - Track Energy (kWh), Water (L), and Carbon (kg CO₂) usage
- **Data Visualization** - Interactive charts using Chart.js for trend analysis
- **AI Insights** - Personalized recommendations using Hugging Face API
- **Modern UI** - Beautiful, responsive design with Tailwind CSS

## 🛠 Tech Stack

### Frontend
- React + Vite
- Tailwind CSS
- Chart.js
- Axios
- Firebase Authentication
- React Router

### Backend
- Node.js + Express
- MongoDB Atlas
- Hugging Face Inference API

## 📁 Project Structure

```
green-intelligence/
├── client/          # React frontend
│   ├── src/
│   │   ├── pages/    # Login, Dashboard, Energy, Water, Carbon
│   │   ├── components/ # Reusable components
│   │   └── ...
│   └── package.json
└── server/          # Express backend
    ├── routes/       # API routes
    ├── models/       # MongoDB models
    └── package.json
```

## 🔧 Setup Instructions

### Prerequisites
- Node.js (v18 or higher)
- MongoDB Atlas account (free tier)
- Firebase project
- Hugging Face account (for API key)

### 1. Backend Setup

```bash
cd server
npm install
```

Create a `.env` file in the `server` directory:

```env
PORT=5000
MONGO_URI=your_mongodb_atlas_connection_string
HF_API_KEY=your_huggingface_api_key
```

Start the server:
```bash
npm start
# or for development with auto-reload
npm run dev
```

### 2. Frontend Setup

```bash
cd client
npm install
```

Create a `.env` file in the `client` directory:

```env
VITE_API_URL=http://localhost:5000
VITE_FIREBASE_API_KEY=your_firebase_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
VITE_FIREBASE_PROJECT_ID=your_firebase_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
VITE_FIREBASE_MESSAGING_SENDER_ID=your_firebase_sender_id
VITE_FIREBASE_APP_ID=your_firebase_app_id
```

Start the development server:
```bash
npm run dev
```

The app will be available at `http://localhost:3000`

## 🔑 Getting API Keys

### Firebase Setup
1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Create a new project
3. Enable Authentication → Email/Password
4. Copy your Firebase config values

### MongoDB Atlas Setup
1. Go to [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
2. Create a free cluster
3. Get your connection string
4. Replace `<password>` with your database password

### Hugging Face Setup
1. Go to [Hugging Face](https://huggingface.co/)
2. Create an account
3. Go to Settings → Access Tokens
4. Create a new token with read permissions

## 📱 Usage

1. **Sign Up / Login** - Create an account or login with existing credentials
2. **Add Entries** - Track your daily consumption of Energy, Water, and Carbon
3. **View Dashboard** - See totals and recent entries
4. **Explore Resources** - Click on Energy, Water, or Carbon blocks to see detailed charts
5. **Get AI Insights** - Receive personalized recommendations based on your usage

## 🚢 Deployment

### Frontend (Vercel)
1. Push code to GitHub
2. Import project in Vercel
3. Add environment variables
4. Deploy

### Backend (Render)
1. Create a new Web Service
2. Connect your GitHub repository
3. Set build command: `cd server && npm install`
4. Set start command: `cd server && npm start`
5. Add environment variables
6. Deploy

## 🎨 Design

- **Primary Green:** #2C7A2C
- **Light Background:** #F4FFF4
- **Accent:** #E6FFE6
- **Font:** Inter / Poppins

## 📝 API Endpoints

- `POST /api/entry/add` - Add a consumption entry
- `GET /api/entry/recent/:email` - Get recent entries
- `GET /api/entry/:type/:email` - Get entries by resource type
- `POST /api/insight` - Generate AI insights

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open source and available under the MIT License.

---

**Made with 🌿 for a sustainable future**


