🛠️ Chat CLI with AI Integration

A Python-based command-line chat application powered by AI models. It uses a local SQLite database to store chat history and supports multiple models via an API.

📂 Project Structure

├── chat_cli.py            # CLI interface for interacting with the chat system  
├── main.py                # Main entry point to run the application  
├── database.py            # Database management for storing chat history  
├── config.yaml            # Configuration file for API keys and settings  
└── models.yaml            # List of available models with descriptions  

⚙️ Setup Instructions
	1.	Clone the repository:

git clone https://github.com/your-repo/chat-cli.git  
cd chat-cli

	2.	Create a virtual environment (optional but recommended):

python -m venv venv  
source venv/bin/activate    # On Windows, use `venv\Scripts\activate`

	3.	Install dependencies:
Create a requirements.txt file (if not provided) and install the necessary libraries:

pip install -r requirements.txt

	4.	Configure the API:
Update config.yaml with your API key:

api_key: "PASTE YOUR API KEY HERE PLEASE!!!!"  
base_url: "https://openrouter.ai/api/v1"  
database_file: "chat_history.db"  
default_model: "google/gemini-2.0-flash-lite-preview-02-05:free"  
history_file: ".chat_history"

	5.	Run the application:

python main.py

🛠️ Features
	•	AI-Powered Chat:
Interact with different AI models through the CLI.
	•	Model Switching:
Choose from multiple models listed in models.yaml:
	•	Gemini Flash Light
	•	Gemini 2.0 Flash Thinking
	•	Gemini 2.0 Pro
	•	DeepSeek R1
	•	Chat History:
Save and load previous conversations automatically using SQLite.
	•	Configurable Settings:
Easily manage API keys, base URLs, and default models with config.yaml.

🚀 Example Usage
	1.	Start the chat:

python main.py

	2.	Choose a model:

Select a model:  
1. Gemini Flash Light  
2. Gemini 2.0 Pro  
3. DeepSeek R1  

	3.	Chat with the AI:

You: Hello, how are you?  
AI: I’m doing great! How can I assist you today?  

	4.	Exit and resume later:
Your chat history will be saved automatically.

🛠️ Customization

Want to add more models? Just edit models.yaml:

- name: "new-ai-model"  
  description: "Description of the new model"

And update your config.yaml if needed!

📘 Future Improvements
	•	Error Handling: Better feedback for API errors or invalid input.
	•	Web UI: Extend the CLI to a web app using Flask or FastAPI.
	•	Model Comparison: Support querying multiple models simultaneously for comparison.
	•	File Uploads: Enable the chat to process and understand uploaded files.

