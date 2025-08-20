# hack-o-week
AI Chatbot for health support
Tech Stack
Our technology choices are focused on speed and power, which is ideal for a hackathon.
Backend: We're using Python with the FastAPI framework. This makes our server very fast and easy to build.
AI / NLP: The core of our chatbot is powered by Hugging Face Transformers. We are using a pre-trained model to understand the emotions in the user's messages without needing to train our own.
Frontend: The user interface is built with standard HTML, CSS, and JavaScript. This keeps it simple and ensures it runs in any browser.
Database: For storing responses, we are using a simple JSON file. It's lightweight and perfect for this project's scope.
Workflow
Here’s how the application works from start to finish:
User Sends a Message: You type a message into the chat window in your browser and hit send.
Frontend to Backend: The JavaScript on the webpage sends your message to our Python backend server.
Crisis Check: The very first thing the server does is check your message for any urgent, high-risk keywords. If it finds any, it immediately sends back a crisis support message with helpline numbers.
AI Emotion Analysis: If no crisis words are found, your message is sent to the Hugging Face AI model, which analyzes it and identifies the primary emotion (like sadness or fear).
Tiered Response: Based on the emotion detected, the system chooses the right level of response: a gentle, supportive message (Tier 1) or a message with specific, helpful resources (Tier 2).
Backend to Frontend: The server sends the chosen response back to the webpage.
Reply Displayed: The JavaScript code displays the AI's message in the chat window for you to see.


