1. git clone -b Multi-AI-Agent-OpenAI-Agent-SDK https://github.com/Noor-Khial/Multi-AI-Agent-OpenAI.git

2. copy sample.env to .env and update

3. python -m venv venv

4. .\venv\Scripts\activate

5. python -m pip install -r requirements.txt

6. chainlit run app.py

The Triage Agent initially handles the request.
Based on the user’s input, the Triage Agent delegates the request to the appropriate specialized agent (FAQ, Account Management, or Live Agent).
The selected agent processes the request using its defined tools and instructions.
Responses are streamed back to the user interface.
After processing, temporary conversation threads are cleaned up, and new threads are created for subsequent interactions.
