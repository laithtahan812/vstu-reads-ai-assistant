VSTU READS AI Assistant

VSTU READS AI Assistant is a Telegram-based AI assistant developed to support a graduation project on Russian-language text analysis and thematic grouping.

The bot answers questions about the diploma project, including the project topic, goal, relevance, architecture, modules, technologies, database structure, testing, effectiveness, and future development.

Project Topic

Development of a system for analyzing Russian-language texts with the identification of thematic groups.

Russian title:

«Разработка системы анализа русскоязычных текстов с выделением тематических групп»

Purpose of the Bot

The Telegram bot was created as an additional AI assistant for explaining and presenting the graduation project. It helps quickly answer questions related to the VSTU READS system and supports preparation for project defense.

The bot does not replace the main VSTU READS desktop application. It works as a reference assistant that explains the project structure and logic.

Main Application: VSTU READS

VSTU READS is a desktop application designed for analyzing Russian-language texts. The system allows users to:

* enter or upload Russian-language text;
* perform text preprocessing;
* identify keywords;
* determine the thematic group of the text;
* save analysis results;
* view history;
* display analytical charts;
* export reports to PDF.

Bot Features

The Telegram bot can answer questions about:

* the topic and goal of the graduation project;
* project relevance;
* object and subject of research;
* system tasks;
* system architecture;
* main modules of VSTU READS;
* technologies used in the project;
* database structure;
* text analysis algorithm;
* testing results;
* system effectiveness;
* future development prospects.

Technologies Used

The bot was developed using:

* Python;
* python-telegram-bot;
* Telegram Bot API;
* Ollama;
* local language model;
* knowledge_base.txt as the project knowledge base;
* dotenv for environment variables.

The main VSTU READS application uses:

* Python;
* PySide6;
* SQLite;
* Matplotlib;
* Visual Studio Code;
* PDF export tools;
* text processing libraries.

Why Ollama Is Used

Ollama is used to run a local language model without relying on a paid external API. This allows the bot to work locally and answer project-related questions using the prepared knowledge base.

Project Structure

vstu-reads-ai-assistant/
│
├── bot.py
├── knowledge_base.txt
├── requirements.txt
├── README.md
├── .gitignore
└── .env

The .env file is not included in the GitHub repository because it contains private configuration data such as the Telegram bot token.

Environment Variables

Create a .env file in the project folder and add:

TELEGRAM_BOT_TOKEN=your_telegram_bot_token_here
OLLAMA_MODEL=llama3.2:3b

Installation

Clone the repository:

git clone https://github.com/laithtahan812/vstu-reads-ai-assistant.git
cd vstu-reads-ai-assistant

Create and activate a virtual environment:

python3 -m venv .venv
source .venv/bin/activate

Install dependencies:

python3 -m pip install -r requirements.txt

Install and run Ollama, then pull the model:

ollama pull llama3.2:3b

Run the bot:

python3 bot.py

Example Questions

The bot can answer questions such as:

Какая тема моей ВКР?
Какая цель моей ВКР?
Почему тема моей ВКР актуальна?
Какие модули есть в VSTU READS?
Какие технологии используются?
Какая архитектура у системы?
Какие таблицы есть в базе данных?
Как работает алгоритм анализа текста?
Как тестировалась система?
Какая эффективность системы?
Зачем нужен Telegram-бот?
Почему бот использует Ollama?

Security Notice

The Telegram bot token must be stored only in the .env file. It should not be uploaded to GitHub.

The repository includes .gitignore to prevent uploading private files such as:

.env
.venv/
__pycache__/
*.pyc
.DS_Store

Author

Laith Tahan

Graduation project: VSTU READS — Russian-language text analysis system with thematic grouping.