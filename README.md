# Jarvis-AI virtual assistant using python

This code implements a basic virtual assistant named "Jarvis" using Python. The assistant can perform various tasks such as greeting the user, searching Wikipedia, opening websites, playing music, telling the time, opening applications, and sending emails. It uses several Python libraries for speech recognition, text-to-speech, and other functionalities.

# Features
1. Text-to-Speech (TTS): Uses pyttsx3 to convert text to speech.Configured to use a specific voice (SAPI5 engine).

2. Speech Recognition: Uses speech_recognition to capture and recognize spoken commands from the user.Processes audio input via a microphone.

3. Greeting Function: Greets the user based on the current time of day (morning, afternoon, evening).Introduces itself as "Jarvis".

4. Wikipedia Search: Searches Wikipedia for a given query and reads out a brief summary.

5. Web Browser Control: Opens popular websites such as YouTube, Google, and Stack Overflow.

6. Music Playback: Plays music from a specified directory on the user's computer.

7. Time Announcement: Announces the current time.

8. Application Launching: Opens Visual Studio Code.

9. Email Sending: Sends an email to a specified recipient using Gmail's SMTP server.

# How to Use
1. Setup: Ensure you have Python installed on your system.

   Install the required libraries using pip:
   Copy code: pip install pyttsx3 speechRecognition Wikipedia

   Replace placeholders with your own email and password for the email functionality.

2. Running the Program: Run the Python script.
Jarvis will greet you based on the time of day.

3. Interacting with Jarvis: Speak your command clearly into the microphone.
Jarvis will recognize and process your command.
Examples of commands you can use:
"Search Wikipedia for [query]"
"Open YouTube"
"Open Google"
"Play music"
"What is the time?"
"Open code"
"Email to Harry"

# Description
The code initializes the pyttsx3 text-to-speech engine and sets the voice property. It defines several functions:

speak(audio): Converts text to speech.
wishMe(): Greets the user based on the time of day.
takeCommand(): Listens to the user's voice command and converts it to text.
sendEmail(to, content): Sends an email using SMTP.
The main function starts by calling wishMe() to greet the user. It then enters an infinite loop, where it continuously listens for commands. Based on the recognized command, it performs the corresponding action such as searching Wikipedia, opening a website, playing music, announcing the time, launching an application, or sending an email.

In case of email functionality, it catches any exceptions and informs the user if the email could not be sent. This virtual assistant provides a hands-free way to perform various tasks through voice commands.
