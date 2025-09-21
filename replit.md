# NexoraX AI - Replit Setup

## Project Overview
NexoraX AI is a modern Vietnamese AI chat application that provides conversations using Google Gemini language model. Successfully imported and configured for Replit environment on September 18, 2025.

## Recent Changes
- **September 20, 2025**: Fixed mobile UI issues
  - **Send Button Mobile Fix**: Increased touch target size from 22px to 40px for better touch interaction
  - **Input Bar Mobile Fix**: Enhanced mobile keyboard behavior with better focus/blur handling
  - **Touch Events**: Added touchend event handling alongside click events for improved mobile responsiveness
  - **Mobile Layout**: Improved mobile styling with better spacing and touch-action optimization
  - **Send Button Visibility Fix**: Fixed missing send button by increasing size from 24px to 32px on desktop and changing color from gray to blue for better visibility
- **September 19, 2025**: Enhanced for Google Pro users with unlimited tokens
- **Security**: Restored original API key configuration per user request
- **Token Limits**: Increased maxOutputTokens from 2048 to 8192 tokens
- **Performance**: Extended server timeout from 30 to 120 seconds
- **Error Handling**: Improved API error messages and MAX_TOKENS handling
- **September 18, 2025**: Successfully imported from GitHub and configured for Replit
- Python 3.11 module installed and configured  
- Workflow configured to run on port 5000
- Deployment settings configured for autoscale
- Application tested and verified working
- **Removed Groq API**: Cleaned up codebase to only use Gemini API

## User Preferences
- Vietnamese interface (main target audience)
- Simple, everyday language for communication
- Prefers lightweight, secure solutions

## Project Architecture

### Technology Stack
- **Frontend**: Vanilla JavaScript with TailwindCSS (CDN) and Marked.js (CDN)
- **Backend**: Python 3.12 HTTP server (built-in modules only)
- **Port**: 5000 (single server for both static files and API proxy)
- **Host**: 0.0.0.0 (configured for Replit proxy requirements)

### Current Configuration
- **Workflow**: "NexoraX AI Server" running `python3 server.py`
- **Deployment**: Configured for autoscale deployment target
- **Dependencies**: No external Python packages required (uses built-in modules)

### File Structure
```
/
├── index.html           # Main application interface (Vietnamese)
├── server.py           # Python HTTP server with API proxy
├── config.py           # Configuration (handles secrets gracefully)
├── assets/
│   ├── css/style.css   # Application styles
│   └── js/app.js       # JavaScript application logic
├── attached_assets/    # User uploaded images/files  
├── NexoraX.md           # Original project documentation
├── README_RENDER.md   # Render deployment guide
└── replit.md          # This file
```

### Features Working
✅ Static file serving
✅ Responsive Vietnamese chat interface  
✅ File upload support
✅ Chat history management
✅ Dark/light theme toggle
✅ Mobile-responsive sidebar
✅ Error handling for missing API keys

### API Integration
- **Gemini API**: Ready for GEMINI_API_KEY secret
- **Graceful handling**: App works without keys, shows proper error messages

### Deployment Notes
- Configured for autoscale deployment
- Uses PORT environment variable when deployed
- No build step required (static files + Python server)
- Production-ready CORS and security settings

## Next Steps for User
1. **Add API Keys** (optional): Add GEMINI_API_KEY to Secrets for AI functionality
2. **Deploy**: Use Replit's deploy feature (already configured)
3. **Customize**: Modify branding, colors, or features as needed

## Status
🟢 **READY TO USE** - Application is fully functional and ready for deployment or further customization.