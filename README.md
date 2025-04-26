# Agentic-AI-Video-Summarizer
This is Video-Summarizer build with Agents of PHIDATA.

Dependencies and Setup:
The code uses several important libraries:
streamlit for creating the web interface
phi for AI agent functionality
google.generativeai for Gemini AI integration
dotenv for environment variable management
tempfile for handling temporary video files
Environment Configuration:
The app loads environment variables from a .env file
It specifically looks for a GEMINI_API_KEY which is required for the Gemini AI service
The API key is configured for the Gemini service
Streamlit UI Setup:
The page is configured with:
Title: "Multimodal AI Agent- Video Summarizer"
Icon: 🎥
Layout: Wide format
The main title and header are set with emojis for visual appeal
AI Agent Initialization:
An agent is created using the @st.cache_resource decorator for caching
The agent uses:
Gemini 2.0 Flash Exp model
DuckDuckGo as a tool for web research
Markdown support for formatted responses
Main Application Features:
File Upload:
Users can upload video files (mp4, mov, avi formats)
The uploaded video is temporarily stored and displayed in the interface
User Query Interface:
A text area for users to input their questions about the video
Help text guides users on what to ask
Analysis Process:
When the "Analyze Video" button is clicked:
The video is uploaded to Gemini's service
The system waits for video processing
Creates a detailed analysis prompt
Uses the AI agent to analyze the video and answer the user's query
Displays the results in a formatted way
Error Handling and Cleanup:
Comprehensive error handling for the analysis process
Automatic cleanup of temporary video files
User-friendly error messages
UI Customization:
Custom CSS to adjust the text area height
Informative messages and warnings for user guidance
Key Features:
Video analysis with AI
Web research integration
Markdown-formatted responses
User-friendly interface
Secure API key management
Temporary file handling
Error handling and cleanup
This application essentially creates an intelligent video analysis tool that can:
Accept video uploads
Process them using Gemini AI
Answer specific questions about the video content
Provide additional context through web research
Present results in a user-friendly format
The code follows good practices like:
Environment variable management
Resource caching
Proper error handling
Cleanup of temporary files
User-friendly interface design
Clear documentation and help text
