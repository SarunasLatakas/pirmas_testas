##Mano įžvalgos
Darant sveikatingumo aplikaciją, nepavyko užkurti nei vieno iš Gemmos modelių. Išmetė error'ą dėl galimai ušnaudotų accounto kreditų. Galiausiai suveikė naudojant Qwen3 14B. Manau geriausia būtų naudoti online LLMus, kurie nesisuka lokaliai ir nevalgo kompiuterio resursų.

# Health & Fitness Coach Application

## How to Run the Application

### 1. Activate the Virtual Environment

**On macOS/Linux:**
```bash
source venv/bin/activate
```

**On Windows:**
```bash
venv\Scripts\activate
```

### 2. Run the Streamlit Application

```bash
streamlit run app.py
```

The application will automatically open in your default web browser at `http://localhost:8501`

### 3. Using the Application

1. **Enter your OpenRouter API Key** in the sidebar to use Qwen3 14B
   - Get your API key from [OpenRouter](https://openrouter.ai/)
   
   2. **Fill in your information:**
   - Age (must be a number)
   - Known health issues
   - Daily exercise time in minutes
   - Fitness goal (Lose weight or Gain muscle)
   
3. **Click "Generate My Exercise Plan"** to receive your personalized weekly workout plan

4. **Download the plan** using the download button if you want to save it

### Features

✅ User-friendly web interface
✅ Multiple AI model options
✅ Input validation (age must be numbers)
✅ Personalized exercise recommendations
✅ Weekly workout plans
✅ Download feature for exercise plans
✅ Professional health and fitness coaching responses
✅ Safety disclaimer included

### Deactivating the Virtual Environment

When you're done, you can deactivate the virtual environment:

```bash
deactivate
```

### Troubleshooting

- **API Key Error**: Make sure you've entered a valid OpenRouter API key
- **Model Error**: Ensure you have credits in your OpenRouter account
- **Age Validation**: Age must be entered as a number (e.g., 25), not text

### Requirements

- Python 3.9+
- streamlit
- openrouter-client-unofficial

All dependencies are already installed in the virtual environment.
