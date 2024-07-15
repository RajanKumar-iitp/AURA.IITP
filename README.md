
# AURA: AI-Powered Desktop Voice Assistant

AURA (Artificially Utilized Responsive Assistant) is an AI-powered desktop voice assistant developed in Python. It integrates several libraries and APIs to deliver a wide range of functionalities, providing an interactive and intelligent user experience. AURA is designed to handle various tasks, from playing music to fetching weather updates and performing web scraping. Below is an extended description of the project's key features and components:

## Key Features

### Voice Interaction
- **Speech Recognition**: Uses `speech_recognition` library to capture and understand voice commands.
- **Text-to-Speech**: Utilizes `gTTS` (Google Text-to-Speech) to convert text responses into spoken words.

### Task Management
- **Task Addition**: Users can add tasks to a CSV file.
- **Task Viewing**: AURA reads out all tasks stored in the CSV file.
- **Task Removal**: Users can remove specified tasks from the CSV file.

### Audio Capabilities
- **Music Playback**: Supports playback of various audio formats (.mp3, .wav, .mpeg, .ogg, .flac).
- **Music Control**: Includes functionalities to play, pause, resume, stop, skip, and rewind tracks.
- **Recording and Playback**: Can record audio from the microphone and playback the recorded audio.

### Online Services Integration
- **Weather Updates**: Fetches weather information for a specified city using the OpenWeather API.
- **News Headlines**: Retrieves the latest news headlines using the News API.
- **Wikipedia Integration**: Provides summaries of Wikipedia articles based on user queries.
- **Web Scraping**: Scrapes websites to extract titles, descriptions, headings, and paragraph texts using `BeautifulSoup`.
- **Joke Fetching**: Delivers jokes using the `pyjokes` library.

### Web Browsing Shortcuts
- Opens commonly used websites such as YouTube, Wikipedia, Google, Spotify, and IIT Patna's official website in the default web browser.

### Date and Time
- Provides the current date and time on request.

### Simple Calculations
- Evaluates basic arithmetic expressions provided by the user.

## Implementation Details

### Libraries and Dependencies
- **`os`**: For file operations and system commands.
- **`datetime`**: To handle date and time functionalities.
- **`sounddevice` and `numpy`**: For recording audio.
- **`speech_recognition`**: For converting speech to text.
- **`gTTS` and `pydub`**: For text-to-speech and audio playback.
- **`webbrowser`**: To open URLs in the default web browser.
- **`threading`**: To handle music playback in a separate thread.
- **`wikipedia`**: To fetch Wikipedia article summaries.
- **`pyjokes`**: To fetch jokes.
- **`BeautifulSoup` and `requests`**: For web scraping.
- **`csv`**: To handle task management using CSV files.

### API Keys
- **Weather API**: Uses OpenWeather API with a specific API key.
- **News API**: Uses News API with a specific API key.

### Music Playback
- Music files are retrieved from a specified folder, and the assistant can play, pause, resume, stop, skip, and rewind tracks using threading to manage playback without blocking other operations.

### Main Function
The `main` function initializes the task file and enters a loop to continuously listen for user commands. Based on the recognized commands, AURA performs the appropriate actions.

```python
if __name__ == "__main__":
    main()
```

### Future Enhancements
Future plans for AURA include:
- Integrating with smart home devices.
- Exploring applications in healthcare and education.
- Implementing adaptive learning through machine learning.
- Developing a graphical user interface (GUI) for a more user-friendly experience.

AURA is a comprehensive project showcasing the power of AI and voice interaction in creating responsive and interactive desktop assistants. It combines various technologies and libraries to offer a rich set of features, making it a valuable tool for daily tasks and entertainment.
