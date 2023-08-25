import speech_recognition as sr
#pip install pyaudio

# Initialize the recognizer
recognizer = sr.Recognizer()

# Record audio from the microphone
with sr.Microphone() as source:
    print("Say something:")
    audio = recognizer.listen(source)

    # Recognize the speech
try:
    text = recognizer.recognize_google(audio)
    print("You said:", text)
    print()

except sr.UnknownValueError:
    print("Sorry, could not understand audio.")
    print()

except sr.RequestError as e:
    print("Error requesting results from Google Speech Recognition service; {0}".format(e)) 
