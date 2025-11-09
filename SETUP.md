# 🚀 Quick Setup Guide

## Step 1: Install Dependencies

### Backend
```bash
cd server
npm install
```

### Frontend
```bash
cd client
npm install
```

## Step 2: Configure Environment Variables

### Server (.env file in `server/` directory)
```env
PORT=5000
MONGO_URI=mongodb+srv://username:password@cluster.mongodb.net/green-intelligence?retryWrites=true&w=majority
HF_API_KEY=your_huggingface_api_key_here
```

### Client (.env file in `client/` directory)
```env
VITE_API_URL=http://localhost:5000
VITE_FIREBASE_API_KEY=your_firebase_api_key
VITE_FIREBASE_AUTH_DOMAIN=your-project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your-project-id
VITE_FIREBASE_STORAGE_BUCKET=your-project.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=123456789
VITE_FIREBASE_APP_ID=1:123456789:web:abcdef
```

## Step 3: Get Your API Keys

### Firebase
1. Go to https://console.firebase.google.com/
2. Create a new project
3. Enable Authentication → Sign-in method → Email/Password
4. Go to Project Settings → General → Your apps → Web app
5. Copy the config values

### MongoDB Atlas
1. Go to https://www.mongodb.com/cloud/atlas
2. Create a free cluster
3. Create a database user
4. Whitelist your IP (or use 0.0.0.0/0 for development)
5. Get connection string from "Connect" → "Connect your application"

### Hugging Face
1. Go to https://huggingface.co/
2. Sign up / Login
3. Go to Settings → Access Tokens
4. Create a new token (read permissions are enough)

## Step 4: Run the Application

### Terminal 1 - Backend
```bash
cd server
npm start
```

### Terminal 2 - Frontend
```bash
cd client
npm run dev
```

Visit http://localhost:3000 in your browser!

## 🎉 You're All Set!

The application should now be running. Create an account and start tracking your sustainability metrics!


