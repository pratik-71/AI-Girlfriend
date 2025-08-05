# AI Chatbot Mobile App

A beautiful, mobile-optimized AI chatbot built with React and Capacitor.js that can be deployed as a native mobile app.

## Features

- 💕 **AI Girlfriend Chatbot** - Human-like conversational AI
- 📱 **Mobile Optimized** - Responsive design for mobile devices
- 🎨 **Beautiful UI** - Modern gradient design with animations
- 🔄 **Memory System** - Remembers conversations and user preferences
- 📱 **Native Mobile App** - Can be built for Android and iOS

## API Configuration

The chatbot uses OpenRouter API for AI responses. To fix the "User not found" error:

### Option 1: Get a Free API Key
1. Visit [OpenRouter.ai](https://openrouter.ai/keys)
2. Sign up for a free account
3. Generate an API key
4. Create a `.env` file in your project root:
   ```
   REACT_APP_OPENROUTER_API_KEY=your_api_key_here
   ```
5. Restart the development server: `npm start`

### Option 2: Use Fallback Mode
The app now includes fallback responses when the API is unavailable, so it will still work even without a valid API key.

### Option 3: Use Your Own API Key
Replace the API key in `src/components/ChatbotLangChain.js`:
```javascript
const apiKey = 'your_api_key_here';
```

## Mobile App Development

This project uses **Capacitor.js** to convert the React web app into native mobile applications.

### Prerequisites

- Node.js and npm
- Android Studio (for Android development)
- Xcode (for iOS development, macOS only)

### Available Scripts

```bash
# Build and sync with mobile platforms
npm run cap:build

# Open Android Studio
npm run cap:android

# Open Xcode (macOS only)
npm run cap:ios

# Run on Android device/emulator
npm run cap:run:android

# Run on iOS device/simulator (macOS only)
npm run cap:run:ios

# Sync changes to mobile platforms
npm run cap:sync
```

### Building for Android

1. Install Android Studio
2. Set up Android SDK
3. Run: `npm run cap:android`
4. Build and run in Android Studio

### Building for iOS (macOS only)

1. Install Xcode
2. Run: `npm run cap:ios`
3. Build and run in Xcode

## Web Development

### Getting Started

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm start
```

3. Build for production:
```bash
npm run build
```

## Project Structure

```
ai_chatbot/
├── src/
│   ├── components/
│   │   └── ChatbotLangChain.js  # Main chatbot component
│   ├── App.js                    # Main app component
│   └── index.js                  # Entry point
├── android/                      # Android native project
├── ios/                         # iOS native project
├── capacitor.config.ts           # Capacitor configuration
└── package.json
```

## Mobile Optimizations

- Responsive design for different screen sizes
- Touch-friendly interface
- Auto-resizing text input
- Mobile-specific UI adjustments
- Native keyboard handling
- Splash screen and status bar integration

## Technologies Used

- **React** - Frontend framework
- **Capacitor.js** - Mobile app framework
- **Tailwind CSS** - Styling
- **LangChain** - AI conversation management
- **Axios** - HTTP requests

## License

This project is for educational purposes.
