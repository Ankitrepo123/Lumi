Lumi: Voice-Activated Personal Assistant
Overview

Lumi is a Python-based voice assistant that listens to user commands, speaks responses, and performs common tasks such as web searches, opening applications, retrieving weather updates, and answering computational questions.

Features

Voice Interaction: Speech recognition and text-to-speech.

Web Actions: Opens YouTube, Google, Gmail, Stack Overflow, or any searched URL.

Information Retrieval:

Wikipedia summaries.

Weather details from OpenWeatherMap API.

Latest headlines from Times of India.

Computational answers via WolframAlpha.

System Functions:

Provides current time.

Takes photos with the camera.

Logs off or shuts down the system.

Requirements

Python 3.x

Packages:

speech_recognition

pyttsx3

wikipedia

webbrowser (standard library)

requests

ecapture

wolframalpha

datetime (standard library)

os, time, subprocess, json (standard library)

Install dependencies:

pip install speechrecognition pyttsx3 wikipedia requests ecapture wolframalpha

Setup

Clone this repository:

git clone <repo_url>
cd <repo_folder>

Obtain API keys:

OpenWeatherMap: Replace api_key in the code with your key.

WolframAlpha: Replace app_id with your WolframAlpha App ID.

Ensure a working microphone and camera are connected.

Usage

Run the assistant:

python virtual.py

Speak commands such as:

“Open YouTube”

“Search machine learning”

“What’s the weather in Delhi?”

“Time”

“Who are you?”

Say “good bye” or “stop” to end the session.

File Structure
virtual.py # Main application script

Notes

Internet connection required for Wikipedia, weather, and WolframAlpha features.

System logoff requires Windows (uses shutdown /l).
