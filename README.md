# 🎥 YouTube Video Summarizer

An AI-powered YouTube Video Summarizer built using **Python, Streamlit, and Google Gemini AI**. This application extracts transcripts from YouTube videos and converts them into concise, meaningful notes with important points in approximately 250 words.

## ✨ Features

- **YouTube Transcript Extraction:** Extracts video transcripts using the YouTube Transcript API.
- **AI-Powered Summarization:** Uses Google Gemini AI to generate summaries from video transcripts.
- **Detailed Notes:** Converts lengthy video transcripts into concise summaries of approximately 250 words.
- **Key Point Extraction:** Presents important information in easy-to-understand bullet points.
- **Video Preview:** Displays the YouTube video thumbnail using its video ID.
- **Interactive Interface:** Simple and user-friendly interface built with Streamlit.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Backend programming |
| Streamlit | Web application interface |
| Google Gemini AI | AI-powered text summarization |
| YouTube Transcript API | Extracting YouTube video transcripts |
| Python-dotenv | Managing environment variables |

## 📁 Project Structure

```text
ytvideo_transcriber/
│
├── app.py              # Main Streamlit application
├── requirements.txt    # Project dependencies
├── .env                # API key configuration (not uploaded)
├── .gitignore          # Files excluded from Git
└── README.md           # Project documentation
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/ytvideo_transcriber.git
```

### 2. Navigate to the Project Directory

```bash
cd ytvideo_transcriber
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

**Windows:**

```powershell
venv\Scripts\activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Configure the Gemini API Key

- Visit [Google AI Studio](https://aistudio.google.com/apikey).
- Generate your Google Gemini API key.
- Create a `.env` file in the project root directory.
- Add the following configuration:

```env
GOOGLE_API_KEY=your_google_gemini_api_key
```

Replace `your_google_gemini_api_key` with your actual API key.

**Important:** Never upload your `.env` file or expose your API key publicly.

### 7. Run the Application

```bash
streamlit run app.py
```

The application will open in your default browser, usually at:

```text
http://localhost:8501
```

## 🚀 How to Use

1. Launch the application.
2. Enter a valid YouTube video URL in the input field.
3. View the corresponding YouTube video thumbnail.
4. Click the **Get Detailed Notes** button.
5. The application extracts the video's transcript.
6. Google Gemini AI processes the transcript and generates a concise summary.
7. View the generated detailed notes in the application.

## 📦 Dependencies

The project uses the following Python libraries:

```text
youtube-transcript-api
streamlit
google-generativeai
python-dotenv
```

Install all dependencies using:

```bash
pip install -r requirements.txt
```

## ⚠️ Limitations

- The YouTube video must have an accessible transcript.
- Videos without available captions or transcripts cannot be summarized.
- An active internet connection is required.
- A valid Google Gemini API key is required.
- Summary generation depends on the availability and usage limits of the Gemini API.

## 🔮 Future Enhancements

- Support for multiple transcript languages.
- Download generated notes as PDF or TXT files.
- Generate chapter-wise summaries.
- Extract important keywords and concepts.
- Provide customizable summary lengths.
- Improve the user interface and add summary history.

## 👩‍💻 Author

**Aishwarya Gupta**

---

⭐ If you find this project useful, consider giving the repository a star!
