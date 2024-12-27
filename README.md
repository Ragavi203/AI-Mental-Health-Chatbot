AI POWERED MENTAL HEALTH CHATBOT

Project Overview: This is an AI-driven chatbot designed to assist users by analyzing their emotional state and providing supportive, context-aware responses. The bot uses natural language processing (NLP) techniques to classify emotions such as anxiety, depression, anger, fear, and joy. Additionally, it integrates with the YouTube API to suggest relevant resources for managing emotions.

This project demonstrates the implementation of sentiment analysis, emotion detection through regular expressions, and interaction flow management for mental health support. The bot can engage in empathetic conversations, recommend coping strategies, and deliver personalized resources, all powered by Python-based libraries and APIs.

Technical Features:

Emotion Detection and Sentiment Analysis:
TextBlob is used to perform sentiment analysis on user input, providing polarity scores that indicate the intensity of emotions (positive, neutral, negative).
Emotion detection is carried out using regular expressions to match specific emotion keywords in the input text (e.g., "anxious", "depressed", "happy").
The bot categorizes emotions into predefined classes (e.g., anxiety, depression, joy) based on keyword matching.

Personalized Responses and Coping Suggestions:
Upon detecting the primary emotion, the bot generates responses tailored to the user's emotional state.
Coping mechanisms and suggestions are recommended for emotions like anxiety or depression.
The bot maintains context by storing conversation history, providing a personalized flow and adapting based on the ongoing exchange.

YouTube API Integration:
The bot interacts with the YouTube Data API to fetch videos related to managing emotions. This provides users with external resources, such as guided meditation or stress relief techniques.
The API query is dynamically generated based on the detected emotion, ensuring the recommendations are contextually relevant.

State Management:
The bot tracks user emotional states throughout the conversation using a deque to store the last 20 exchanges. This allows the bot to maintain context over time and provide more nuanced responses.
The bot also tracks the user’s previous emotional states, allowing it to adapt the conversation based on the user’s mental health progress.

Session Management:
The bot tracks the start time of the session, allowing it to provide a sense of continuity and manage the user’s experience effectively.

Technical Architecture:

Emotion Analysis Pipeline:
TextBlob for sentiment analysis to detect polarity and intensity of emotions.
Regex patterns to map emotional keywords and assign primary emotions.

API Integration:
YouTube API for fetching video resources related to mental health topics based on user emotion.

Stateful Conversations:
A deque is used to store the latest 20 conversational exchanges, providing an efficient way to manage state without excessive memory usage.

Response Generation:
Based on the detected emotion, a response is dynamically generated using pre-defined templates. Additional coping strategies and YouTube links are appended to these responses for more in-depth support.

![image](https://github.com/user-attachments/assets/35ef5bd5-c56c-4081-8f75-894155d3513e)
