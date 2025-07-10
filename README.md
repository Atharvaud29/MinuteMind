# 🧠 MinuteMind

**An open-source, privacy-focused Meeting Intelligence Engine for real-time task extraction, conflict detection, and scheduling from audio or transcript data.**

![MinuteMind Banner](https://your-image-url-if-any)

---

## 🚀 Project Overview

Meetings are essential—but often unstructured and hard to follow up on. **MinuteMind** transforms raw audio or transcript files into **clear, actionable insights** using AI models like **WhisperX** and **Phi-3 Mini**, entirely offline.

The system extracts:
- 📌 **Tasks** with deadlines and owners
- ⚠️ **Conflicts** and points of disagreement
- 📅 **Schedule references** like "next Friday" and converts them into calendar entries

Built using **open-source tools** with a focus on **privacy, customizability, and offline deployment**.

---

## 🏗️ Features

- 🎙️ **Audio-to-Text** with speaker diarization using WhisperX
- 🧠 **Task Extraction** using Phi-3 Mini and prompt engineering
- 🔍 **Conflict Detection** via stance/sentiment analysis
- 🕓 **Time Expression Parsing** into ISO datetime
- 🖥️ **Interactive Dashboard** using Streamlit
- 📤 **Data Export** in `.json`, `.txt`, and `.ics` formats
- 🧩 **Modular Architecture** for easy customization
- 🔒 **Fully Local** & Privacy-First (no cloud dependency)

---

## 📂 Project Structure

MinuteMind/
├── data/
│ ├── raw_audio/
│ └── transcripts/
├── src/
│ ├── transcription/
│ ├── preprocessing/
│ ├── extraction/
│ ├── storage/
│ └── utils/
├── frontend/
│ ├── app.py
│ └── components/
├── models/
│ ├── phi3_mini/
│ └── whisperx/
├── exports/
├── requirements.txt
├── config.yaml
└── README.md

▶️ Usage
1. Launch Streamlit Dashboard

Copy code
        streamlit run frontend/app.py


2. Upload Your Meeting Audio / Transcript

Supported formats:

- .mp3, .wav, .m4a (audio)

- .txt or .json (transcripts)

3. Explore Insights

- View extracted tasks, conflicts, and schedules

- Filter by owner, deadline, or conflict

- Edit or export data

🧠 Models Used

| Component              | Model        | Description                        |
| ---------------------- | ------------ | ---------------------------------- |
| Speech-to-Text         | WhisperX     | Accurate ASR + speaker diarization |
| Language Understanding | Phi-3 Mini   | Lightweight LLM for prompt tasks   |
| Time Parsing           | `dateparser` | Converts fuzzy dates to datetime   |


📄 License

- This project is open-source under the MIT License.

👥 Team

- Atharv Yeole

- Atharva Deshmukh

- Arjun Kallurkar

Guide: Dr. Vaishali Y. Baviskar

G H Raisoni College of Engineering and Management, Pune

📌 References
Based on research from:

- Zhang et al. (Structure-aware Dialogue Act Classification)

- Shen et al. (MeetingBank with GPT-4)

- Liu et al. (Task-Aware Summarization)

- Pandya & Gawande (Automatic MOM Generation)