# MOM_generator_HuggingFace
A Minutes of Meeting generator using HuggingFace open source models. Audio-Text-MOM.
# 🤖 Minutes of Meeting Generator using Hugging Face + Whisper

This project is a smart **Meeting Minutes Generator** that takes in an audio file (e.g., a recording of a meeting), converts it into text using **Whisper by OpenAI**, and then uses a **Hugging Face transformer model** (LLama-3 based) to generate structured, professional **Minutes of the Meeting (MoM)** in Markdown format.

---

## 🧠 What it does

1. 🔊 **Speech to Text**:
   - Converts a `.mp3` or other supported audio file to text using `openai/whisper-medium`.

2. 📝 **Meeting Summary Generation**:
   - Transcribes the audio into text.
   - Summarizes the content into minutes, including:
     - Summary with attendees, date, and location
     - Key discussion points
     - Takeaways
     - Action items with owner assignments

3. 📄 **Outputs**:
   - Markdown-formatted **readable minutes** directly usable in documentation.

---

## 🧾 Sample Output

> ✅ Sample result (generated `README` style minutes):

```markdown
### 📍 Meeting Summary
- **Location**: Denver Council Hall
- **Date**: [Extracted from audio or inferred]
- **Attendees**: [Names as per transcript if available]

---

### 🗣️ Key Discussion Points
- Urban development projects in downtown Denver.
- Budget allocation for public parks.
- Feedback from local communities.

---

### ✅ Takeaways
- Budget approval pending council majority.
- Next steps include survey rollout in 2 weeks.

---

### 📌 Action Items
| Task | Owner | Deadline |
|------|-------|----------|
| Prepare budget draft | John Doe | 2024-07-01 |
| Conduct community survey | Jane Smith | 2024-07-15 |
