# G-One: Personal AI Assistant

A Python-based voice-activated personal assistant that listens to user commands, speaks responses, and performs various tasks including web searches, weather updates, computational questions, and system operations.

## 🚀 Features

### Voice Interaction
- **Speech Recognition**: Listens to voice commands using Google's speech recognition
- **Text-to-Speech**: Responds with natural voice using pyttsx3
- **Multi-language Support**: Configured for English (India) dialect

### Web Actions
- **YouTube**: Opens YouTube in your default browser
- **Google**: Opens Google search engine
- **Gmail**: Opens Gmail web interface
- **Stack Overflow**: Opens Stack Overflow login page
- **Custom Search**: Opens any URL you specify

### Information Retrieval
- **Wikipedia**: Provides Wikipedia summaries for any topic
- **Weather**: Real-time weather information for any city worldwide
- **News**: Latest headlines from Times of India
- **Computational Questions**: Answers complex questions using WolframAlpha API

### System Functions
- **Time**: Provides current time
- **Camera**: Takes photos using your webcam
- **System Control**: Logs off or shuts down your system
- **Personalized Greetings**: Time-based greetings (Good Morning/Afternoon/Evening)

## 📋 Requirements

### System Requirements
- **Python 3.x**
- **Windows OS** (uses SAPI5 for text-to-speech)
- **Microphone** for voice input
- **Webcam** (optional, for camera features)
- **Internet Connection** (for API features)

### Python Packages
```
SpeechRecognition
pyttsx3
wikipedia
ecapture
wolframalpha
requests
```

## 🛠️ Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd Personal-ai
   ```

2. **Create a virtual environment (recommended):**
   ```bash
   python -m venv env
   env\Scripts\activate  # On Windows
   ```

3. **Install dependencies:**
   ```bash
   pip install SpeechRecognition pyttsx3 wikipedia ecapture wolframalpha requests
   ```

4. **API Setup:**
   - **OpenWeatherMap**: Replace the `api_key` in `virtual.py` (line 101) with your API key
   - **WolframAlpha**: Replace the `app_id` in `virtual.py` (line 167) with your App ID

## 🎯 Usage

1. **Run the assistant:**
   ```bash
   python virtual.py
   ```

2. **Voice Commands Examples:**
   - `"Open YouTube"` - Opens YouTube
   - `"Search machine learning"` - Opens search results
   - `"What's the weather in Delhi?"` - Gets weather information
   - `"Time"` - Shows current time
   - `"Who are you?"` - Assistant introduction
   - `"Take a photo"` - Captures image from webcam
   - `"Wikipedia artificial intelligence"` - Wikipedia search
   - `"Ask what is the capital of France?"` - Computational question
   - `"Good bye"` or `"Stop"` - Exits the assistant

## 📁 Project Structure

```
Personal-ai/
├── virtual.py          # Main application script
├── requirments.txt     # Python dependencies
├── README.md          # Project documentation
└── env/               # Virtual environment (if created)
```

## 🔧 Configuration

### Voice Settings
The assistant uses a female voice by default. To change the voice:
```python
voices = engine.getProperty('voices')
engine.setProperty('voice', voices[0].id)  # Change index for different voices
```

### API Keys
- **OpenWeatherMap**: Get your free API key from [OpenWeatherMap](https://openweathermap.org/api)
- **WolframAlpha**: Get your App ID from [WolframAlpha](https://developer.wolframalpha.com/)

## ⚠️ Important Notes

- **Internet Required**: Wikipedia, weather, and WolframAlpha features require internet connection
- **Windows Specific**: System logoff feature uses Windows-specific commands (`shutdown /l`)
- **Microphone Access**: Ensure your microphone permissions are enabled
- **API Limits**: Be aware of API rate limits for weather and WolframAlpha services

## 🐛 Troubleshooting

### Common Issues
1. **Microphone not working**: Check microphone permissions and ensure it's not being used by other applications
2. **Speech recognition errors**: Ensure stable internet connection for Google's speech recognition service
3. **API errors**: Verify your API keys are correct and have sufficient quota
4. **Voice not working**: Check if SAPI5 is available on your Windows system

### Error Messages
- `"Pardon me, please say that again"` - Speech recognition failed, try speaking more clearly
- `"City Not Found"` - Weather API couldn't find the specified city
- `"No direct result found"` - WolframAlpha couldn't answer the computational question

## 👨‍💻 Developer

**Created by:** Mr. Ankit Kumar

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📞 Support

If you encounter any issues or have questions, please open an issue in the repository.

---

**Note**: This is a personal AI assistant project designed for educational and personal use. Make sure to respect privacy and security guidelines when using voice recognition features.