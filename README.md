# InlignTech-Python-Project
A Python-based voice assistant that takes voice commands to perform everyday desktop tasks like opening websites, searching Wikipedia, playing music, telling the time, and more. It uses speech_recognition for capturing voice, pyttsx3 for text-to-speech, and integrates system-level controls and web automation.

Project Objectives
To build an intelligent desktop assistant capable of understanding and processing voice commands.
To demonstrate the integration of Python libraries and APIs in creating real-time voice applications.

Methodology
1. Setup and Dependencies
Install and configure required libraries:
speech_recognition – for converting voice to text.
pyttsx3 – for converting text responses to speech.
pyaudio – to access the microphone.
webbrowser, os, datetime, and wikipedia – for system and web tasks.

2. Voice Recognition Input
Use a microphone input with speech_recognition.
The assistant listens continuously or on command.
The captured audio is processed via Google Web Speech API to extract textual commands.

3. Text Parsing and Command Recognition
Convert the captured text to lowercase.
Use if-elif statements to compare the text against pre-defined commands.
Example:
"Open YouTube" triggers webbrowser.open("https://youtube.com")
"What is the time?" uses datetime.datetime.now() and speaks the result.

4. Action Execution
For recognized commands, the assistant executes:
System tasks using os.system() or subprocess.
Web search via the webbrowser module.
Information retrieval using the wikipedia API.
Music playback by accessing a local directory.

5. Voice Feedback
The assistant uses pyttsx3 to provide voice responses.
Responses are dynamic and depend on command type and output.
Example: After fetching data from Wikipedia, the assistant speaks a short summary.

6. Loop and Continuity
The assistant runs in a loop until a termination command (e.g., "exit") is given.
It continues to listen and respond to new inputs, providing an interactive experience.


