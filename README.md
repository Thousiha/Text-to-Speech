This project is a Streamlit web application that converts text to speech using the Google Text-to-Speech (gTTS) library. The application takes user input text, converts it to speech, and allows the user to download the audio file.
Features:

Converts text input to speech
Supports multiple sentences
Offers download functionality for the generated audio
Simple and user-friendly interface
Background animation for an enhanced user experience

Requirements
Python 3.7 or higher
Streamlit
NLTK (Natural Language Toolkit)
gTTS (Google Text-to-Speech)
ffmpeg (for concatenating multiple audio files)

Installation:
Clone the repository:
    git clone https://github.com/your-username/text-to-speech.git
cd text-to-speech

Create a virtual environment (optional but recommended):
python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

Install the required packages:
pip install streamlit nltk gtts

Download NLTK resources:
import nltk
nltk.download('punkt')

Ensure ffmpeg is installed:
sudo apt update
sudo apt install ffmpeg

Running the Application
Run the Streamlit app:

streamlit run app.py
Open your web browser and go to http://localhost:8501 to view the application.

Usage
Enter text: Type or paste the text you want to convert to speech in the text area.
Convert to Speech: Click the "Convert to Speech" button to start the conversion.
Listen and Download: Listen to the generated audio using the audio player provided. You can also download the audio file by clicking the "Download Audio" button

File Structure
app.py: The main application file containing the Streamlit app code.
requirements.txt: A file listing all required Python packages.

Notes
The application uses temporary directories to store intermediate audio files, which are cleaned up after the process is complete.
The concatenation of audio files is handled using ffmpeg.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
The application utilizes the gTTS library for converting text to speech.
Streamlit is used for creating the web application.
Background animations are created using CSS.

Troubleshooting
Ensure that ffmpeg is correctly installed and accessible from your system's PATH.
If you encounter issues with NLTK downloads, ensure you have an active internet connection and correct permissions to write to the NLTK data directory.

Contributing
Feel free to fork the repository and submit pull requests. Contributions are welcome!


