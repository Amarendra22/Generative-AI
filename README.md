# Generative-AI
This is a project on a generative AI which  converts the human voice input to text which is furthur converted to voice using GPT-3.5

### This is a voice-controlled conversational interface that utilizes the Google Speech Recognition API for speech-to-text conversion and the OpenAI GPT-3.5 Turbo model for generating responses.

# Imports that need to be installed
- openai
- pyttsx3
- speech_recognition

### An OpenAI API key needs to be created from the OpenAI's website

Functions:-
transcribe_audio_to_text(filename): Uses the Google Speech Recognition API to transcribe audio from the given filename to text.
generate_response(prompt): Calls the OpenAI GPT-3.5 Turbo model to generate a response based on the given prompt.
speak_text(text): Uses the text-to-speech engine to read out the provided text.

Main Loop:-
Initiates an infinite loop to continuously listen for a specific trigger word ("Smart") using the microphone.
When the trigger word is detected, it records the user's question using the microphone.
The recorded audio is saved to a file named "input.wav".
The recorded audio is transcribed to text using the Google Speech Recognition API.
The transcribed text is used as a prompt to generate a response using the OpenAI GPT-3.5 Turbo model.
The generated response is printed and read out using text-to-speech.
