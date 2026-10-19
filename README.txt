# LegalEase AI - Gemini Version

This version adds Gemini AI document generation to the simple LegalEase application.

## Included
- Gemini AI drafting
- Agreement
- NDA
- Lease Agreement
- Employment Contract
- Employment Offer Letter
- Freelance Contract
- Editable document preview
- TXT/DOCX/PDF downloads
- `.env` API-key configuration

## 1. Install Python
Use Python 3.10+.

## 2. Open Command Prompt
Open CMD inside this project folder.

## 3. Create virtual environment

python -m venv venv

## 4. Activate it on Windows

venv\Scripts\activate

## 5. Install packages

pip install -r requirements.txt

## 6. Configure your Gemini API key

Create a Gemini API key in Google AI Studio.

### Streamlit Community Cloud

Open your app's **Settings > Secrets** and add this TOML entry, replacing the example value with your key:

```toml
GEMINI_API_KEY = "your-gemini-api-key"
```

Save the settings. Streamlit will restart the app and make the key available through `st.secrets`.

### Local development

Either add `GEMINI_API_KEY=your-gemini-api-key` to a `.env` file in the project root, or copy `.streamlit/secrets.toml.example` to `.streamlit/secrets.toml` and replace the example value. The app supports both formats. Both secret files are excluded from Git; never commit or share your real API key.

## 7. Run

streamlit run app.py

Then open http://localhost:8501 if Streamlit does not open the browser automatically.

## API model
The app uses Google's GenAI Python SDK and the Gemini Interactions API with `gemini-3.8-flash`.

## Legal notice
The generated text is a draft. It may contain mistakes or omit requirements of the law applicable to a particular situation. A qualified legal professional should review any document before it is used for an actual legal matter.
