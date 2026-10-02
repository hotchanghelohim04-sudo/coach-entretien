# 🎤 Interview Coach (Coach d'entretien)

An internship interview coach that runs **100% locally** with **Gemma** and **Ollama**.
Built for my friend **Khennel**, a Human Resources student preparing her first internship interviews.

> Built for the DEV **Hacktoberfest Weekend Challenge: Build for a Friend**.
> Category: **Best Use of Gemma**.

## What it does

1. Khennel pastes an internship offer or uploads it (PDF or Word). She can also add her CV.
2. The AI plays the recruiter and asks 10 questions, one at a time, based on the offer (and the CV).
3. At the end, Gemma gives a score out of 10, a summary, strengths, feedback on clarity and structure, and 3 concrete improvements.
4. She can export the results and the full transcript as a Word or text file.

## Why open-source AI?

- **Private:** offers and CVs never leave the laptop.
- **Free:** no API key, no subscription.
- **Works offline** once the model is downloaded.
- **Swappable:** change one line (`MODEL`) to try another Gemma model.

## Run it

1. Install [Ollama](https://ollama.com) and download the model:

   ```
   ollama pull gemma3:4b
   ```

2. Install the dependencies:

   ```
   pip install -r requirements.txt
   ```

3. Start the app:

   ```
   streamlit run app.py
   ```

   On Windows, if `streamlit` is not recognized: `python -m streamlit run app.py`

## Tech stack

- **Gemma** (`gemma3:4b`) through **Ollama**
- **Python** and **Streamlit** (interface)
- `pypdf` and `python-docx` (read PDF/Word files, export Word reports)

## Project files

- `app.py`: the whole application
- `requirements.txt`: Python dependencies

## Settings

At the top of `app.py`:

- `MODEL`: the Gemma model used
- `NB_QUESTIONS`: number of questions asked (default 10)

## Demo

Video: _add the link here_
