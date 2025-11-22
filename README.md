# Chat Space Application

A simple invite-based chat application with server and channel support.

## ⚠️ Important Notes

This is a **frontend-only application** that requires a backend WebSocket server to function properly.

### Backend Requirements

The application expects a WebSocket server running at `wss://your-domain/ws` that handles:
- User authentication (token-based login)
- Server management
- Channel management
- Real-time messaging

### How to Use

1. **Local Development**: 
   - You need a running WebSocket backend server
   - The app will connect to `ws://localhost/ws` when running locally

2. **Production Deployment**:
   - Deploy the frontend to Vercel or similar static hosting
   - Set up and run the backend WebSocket server separately
   - The frontend will attempt to connect to `wss://your-domain/ws`

3. **Authentication**:
   - Users need to log in at `/login/`
   - Credentials are stored in browser localStorage
   - Token-based authentication is used for WebSocket connection

### File Structure

- `index.html` - Main HTML file
- `script.js` - Main application logic
- `client.js` - WebSocket client implementation
- `bar.js` - Navigation bar logic
- `style/dark.css` - Dark theme stylesheet
- `style/index.js` - Theme management

### Features

- 🔐 Token-based authentication
- 🌐 Multiple servers and channels
- 💬 Real-time messaging
- 📊 Ping monitoring
- 🎨 Dark theme

Made by Soft MIDI Player
