# Research Assistant
- A powerful research assistant that leverages AI to process and enhance content. This project features a backend service integrated with the Gemini AI API and a Chrome extension for easy access, allowing users to quickly generate summaries of lengthy texts.

# Project Overview
- The Research Assistant is designed to help users efficiently condense large pieces of text into clear, concise summaries. The backend service builds a custom prompt from the input text, sends it to the Gemini AI API, and returns a well-formulated summary. A dedicated Chrome extension enables you to access these summarization features directly from your browser.

# Features
- Content Summarization: Generate concise summaries from lengthy articles or documents.

- AI Integration: Interacts with the Gemini AI API to produce context-aware summaries.

- Chrome Extension: Offers an intuitive, browser-based interface for quick and easy access.

# Installation & Setup
- Clone the Repository:

- bash
- Copy
- Edit
- git clone https://github.com/yourusername/research-assistant.git
- cd research-assistant
- 
# Backend Setup:
- Ensure you have Java and Maven installed.
- Configure your environment variables or application properties with your Gemini API URL and API key:

# properties
- Copy
- Edit
- gemini.api.url=https://api.gemini.ai/endpoint/
- gemini.api.key=your-gemini-api-key
- Build and run the project:

- bash
- Copy
- Edit
- mvn clean install
- mvn spring-boot:run

# Chrome Extension Setup:

- Open Chrome and navigate to chrome://extensions/.

- Enable Developer mode.

- Click "Load unpacked" and select the chrome-extension directory from the cloned repository.

- The extension should now appear in your browser toolbar.
  

# Usage
Using the Chrome Extension:

- Click the Research Assistant extension icon in your browser toolbar.

- Choose the summarization option.

- Paste or select the text you want to summarize.

- The extension sends the text to the backend service, which processes it and returns a summary.

# Screenshots & Demo:




- A quick demo showing how the Research Assistant processes content via the Chrome extension.

# API Endpoints
The backend service exposes a key endpoint for content summarization:

POST /process
Processes the research content by summarizing the text provided.
Request Body Example:

json-
Copy
Edit
{
  "operation": "summarize",
  "content": "Your text goes here..."
}
# Response Example:

json-
Copy
Edit
{
  "result": "The generated summary."
}

Note: Currently, only the summarization feature is supported.
