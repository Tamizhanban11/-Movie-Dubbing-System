# 🎬 AI Movie Dubbing System

The **AI Movie Dubbing System** is a Python and Streamlit-based application that allows users to upload any movie or video and receive a **dubbed version in their preferred language**. Powered by state-of-the-art speech recognition, translation, and text-to-speech tools, this system automates the end-to-end movie dubbing process.

---

## 🌟 Features

- 🎥 Upload videos in `.mp4`, `.avi`, `.mkv` formats
- 🧠 Transcribe audio using OpenAI's Whisper model
- 🌐 Translate dialogues to any supported language via Google Translate API
- 🗣️ Generate dubbed voice using ElevenLabs (natural-sounding speech)
- 🎞️ Merge dubbed audio with original video using FFmpeg
- 🖥️ Streamlit UI for smooth user experience
- 📥 Download dubbed video directly from the interface

---

## 🛠️ Tech Stack

| Component            | Technology                      |
|---------------------|----------------------------------|
| UI                  | Streamlit                       |
| Speech Recognition  | OpenAI Whisper                  |
| Translation         | Google Translate (via `googletrans`) |
| Text-to-Speech      | ElevenLabs                      |
| Video Processing    | FFmpeg, `moviepy`, `imageio-ffmpeg` |
| Language Support    | English, Spanish, French, German, Hindi, Tamil, Chinese |

---

## 📂 File Structure

movie-dubbing-system/
│
├── app.py # Streamlit UI for uploading and processing
├── dubbing.py # Core logic: transcription, translation, dubbing
├── checkpath.py # Helper to add FFmpeg path to environment
├── temp_movie.mp4 # Placeholder for uploaded video
├── requirements.txt # Project dependencies
├── README.md # Project documentation

yaml
Copy
Edit

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/movie-dubbing-system.git
cd movie-dubbing-system
2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Set Your ElevenLabs API Key
Open dubbing.py and replace:

python
Copy
Edit
set_api_key("your_actual_api_key_here")
with your actual API key from ElevenLabs.

4. Run the App
bash
Copy
Edit
streamlit run app.py
✅ How It Works
Upload a video through the Streamlit interface.

Transcription: The system uses Whisper to convert audio to text.

Translation: The text is translated to the selected target language.

Voice Generation: ElevenLabs converts translated text into realistic voice.

Merging: FFmpeg overlays new audio onto the original video.

Download the final dubbed video.

📈 Future Enhancements
🤖 AI-based lip-syncing

🗃️ User authentication and dubbing history

🌐 Cloud support for large files and multiple users

🧬 Voice cloning to match original speaker

📁 Subtitle export and transcript editing

📜 License
This project is licensed under the MIT License – see the LICENSE file for details.

🙌 Acknowledgements
OpenAI Whisper

Google Translate Python API

ElevenLabs API

FFmpeg

Streamlit
