# ChatGPT Voice Bot

This is a simple voice-capable chatbot that uses the OpenAI ChatGPT API
and its function_call capability to drive another API.

The main program uses ElevenLabs to provide a natural voice response, and
Gradio to create a UI for the bot. It uses the OpenAI `whisper` API
to transcribe the voice to text for the chatbot instructions.

You will require both an OpenAI API key and an ElevenLabs API key for
out-of-the-box functionality.

For a purely text-based chatbot, use `text-chatbot.py`

# Setup

Make sure you have python3 installed:

```
python3 --version
```

Create a virtual environment and install the dependencies:

### Linux/Mac:

```
python3 -m venv venv
. ./venv/bin/activate
pip install -r requirements.txt
```

### Windows:

```
python -m venv venv
venv\Scripts\activate.bat
pip install -r requirements.txt
```

# Configuration

Copy `env.sample` to `.env` and add your OpenAI API key to the file.

```
OPENAI_API_KEY=<<YOUR_API_KEY>>
ELEVENLABS_API_KEY=<<YOUR_ELEVENLABS_API_KEY>>
```

# Running

To run just do the following:

### Linux/Mac:

```
. ./venv/bin/activate
python3 main.py
```

### Windows:

```
venv\Scripts\activate.bat
python main.py
```
