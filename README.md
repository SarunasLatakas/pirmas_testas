## Mano įžvalgos
Darant sveikatingumo aplikaciją, nepavyko užkurti nei vieno iš Gemmos modelių. Išmetė error'ą dėl galimai išnaudotų accounto kreditų. Galiausiai suveikė naudojant Qwen3 14B. Manau geriausia būtų naudoti online LLMus, kurie nesisuka lokaliai ir nevalgo kompiuterio resursų.

# Health & Fitness Coach Application

An AI-powered health and fitness coach application built with Streamlit that provides personalized weekly exercise plans based on user information.

## Features

- 🏋️ Personalized weekly exercise plans
- 🤖 Powered by OpenRouter AI (qwen/qwen3-14b:free model)
- 💪 Tailored recommendations based on:
  - Age and health conditions
  - Available daily exercise time
  - Fitness goals (lose weight or gain muscle)
- ✅ Input validation for user safety
- 📥 Download exercise plans as text files
- ⚠️ Professional disclaimer included

## Installation

### 1. Create a Virtual Environment

```bash
python3 -m venv venv
```

### 2. Activate the Virtual Environment

**On macOS/Linux:**
```bash
source venv/bin/activate
```

**On Windows:**
```bash
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements-install.txt
```

## Usage

### 1. Run the Application

```bash
streamlit run app.py
```

The application will automatically open in your browser at `http://localhost:8501`

### 2. Using the Application

1. **Enter your OpenRouter API Key** in the sidebar
   - Get your free API key from [OpenRouter](https://openrouter.ai/)
   
2. **Fill in your information:**
   - **Age**: Enter your age (must be a number between 1-120)
   - **Known health issues**: List any health conditions or type "None"
   - **Daily exercise time**: How many minutes you can exercise per day
   - **Fitness goal**: Choose either "Lose weight" or "Gain muscle"
   
3. **Generate Plan**: Click "Generate My Exercise Plan" button

4. **Download**: Save your personalized plan using the download button

## Requirements

- Python 3.9+
- streamlit >= 1.50.0
- openrouter-client-unofficial >= 0.0.4

## Project Structure

```
.
├── app.py                      # Main Streamlit application
├── requirements-install.txt    # Python dependencies
├── requirements.txt            # Application requirements document
├── README.md                   # This file
├── HOW_TO_RUN.md              # Detailed running instructions
└── docs/
    ├── models.md              # Model information
    ├── openrouter.md          # OpenRouter documentation
    └── streamlit.md           # Streamlit documentation
```

## Important Notes

⚠️ **Medical Disclaimer**: This application generates AI-based exercise recommendations and should not be treated as professional medical or fitness advice. Always consult with healthcare professionals before starting any new exercise program.

## Troubleshooting

- **API Key Error**: Ensure you've entered a valid OpenRouter API key
- **Model Error**: The application uses the free `qwen/qwen3-14b:free` model
- **Age Validation Error**: Age must be entered as a number (e.g., 25), not letters
- **Virtual Environment**: Make sure the virtual environment is activated before running

## Deactivating Virtual Environment

When finished, deactivate the virtual environment:

```bash
deactivate
```
