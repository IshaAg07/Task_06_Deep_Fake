# 🎙️ Task_06_Deep_Fake – AI-Generated Interview (Syracuse WLAX)

This project is submitted for **Research Task 6: Deep Fake**. It builds upon the narrative developed in **Research Task 5**, which explored descriptive statistics for the 2025 Syracuse Women’s Lacrosse team and evaluated LLM-generated summaries. In this task, we transformed that narrative into an **AI-generated audio interview** using free, open-source tools.

---

## 🎯 Objective

To synthesize a previously generated narrative into a scripted “deep fake” interview — a simulated Q&A between a host and analyst — and convert it into an audio format using free tools. This demonstrates how statistical reasoning and LLM evaluation can be conveyed through voice-driven storytelling.

---

## 🎧 Final Output

- 📁 `final/deepfake_interview.mp3`
- Duration: ~90 seconds
- Format: Host ↔ Analyst audio conversation
- Topic: Syracuse Women’s Lacrosse 2025 season summary, model evaluation, and recommendations

---

## 🛠️ Tools & Workflow

| Tool        | Use Case                                         |
|-------------|--------------------------------------------------|
| gTTS        | Text-to-speech conversion in Python (Colab)      |
| pydub       | Merging audio segments and adding pauses         |
| ffmpeg      | Backend for audio processing                     |
| Google Colab| Code environment (Python 3.12)                   |

---

## 🧪 What Worked / What Didn’t

<pre><code class="language-python">
✅ What Worked
- gTTS: Fast and reliable text-to-speech tool that runs seamlessly in Colab
- pydub: Cleanly merged segments with adjustable silence between speakers
- MP3 output: Clear, distinguishable voices, no API key or login required

❌ What Didn’t Work
- pyttsx3: Requires OS-level TTS engine (e.g., eSpeak), which isn’t available in Colab
- Coqui TTS (`TTS`): Installation failed due to Python 3.12 incompatibility
- ElevenLabs: Considered, but rejected due to account/API requirement and policy preference for free tools
</code></pre>

---

## 🧵 Script Structure (based on Task 5)

- Script reflects findings from our statistical analysis:
  - Game-level stats computed using max(GP)
  - Highlights (top scorer, best shooter)
  - Weaknesses (high TOs)
  - LLM evaluation (ChatGPT vs actual stats)
  - Coaching recommendations
- Script lines located in `script_lines.txt` and `script_lines.py`

---

## 📁 Repository Structure

