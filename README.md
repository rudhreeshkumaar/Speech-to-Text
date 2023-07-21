# Speech to Text Converter
This Python script converts speech to text using the SpeechRecognition library and SoundDevice library. It provides two main functionalities:

Recognizing speech from an existing audio file.
Capturing audio from the microphone and converting it to text.
## Prerequisites
Before running the script, ensure you have the following libraries installed:

SpeechRecognition (pip install SpeechRecognition)
SoundDevice (pip install sounddevice)
SciPy (pip install scipy)
## Usage
Save the script in a Python file, e.g., speech_to_text.py.
Ensure that you have an existing audio file with valid speech data for testing purposes. Update the filename_from_mic variable to specify the path to the file.
Update the filename_result_text variable to set the path and name of the text file where the converted text will be saved.
## Functions
### recognize_from_file(filename)
This function takes the filename of an existing audio file as input and converts the speech in the file to text using the Google Web Speech API. It returns the recognized text.

### recognize_from_microphone(file_to_write)
This function captures audio from the microphone for a duration of 5 seconds, converts it to a WAV format, and saves it to the file specified by file_to_write. Make sure you have a microphone connected to your system to use this functionality.

### save_text_to_file(text, filename)
This function takes the recognized text and saves it to a specified filename in a text file.

## Running the Script
To recognize speech from an existing audio file, uncomment the recognize_from_file(test_filename) function call and replace test_filename with the actual filename.
To capture audio from the microphone and convert it to text, run the script without uncommenting the recognize_from_file(test_filename) function call.
Please note that for the microphone functionality to work, the SoundDevice library must have access to your system's audio input.

## Note
- The script captures audio at a sample rate of 44100 Hz, but you can adjust this value in the recognize_from_microphone() function if needed.
- The recognize_google() function from the SpeechRecognition library uses the Google Web Speech API for speech recognition.
- Ensure you have a stable internet connection for speech recognition from both files and the microphone.
Enjoy using this simple Python script to convert speech to text!
