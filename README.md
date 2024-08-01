<h1 align="center">
  <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
  <br>Discord-Mini-Games-Bot
</h1>
<h3 align="center">◦ A Discord bot for playing engaging mini-games within your server.</h3>
<h3 align="center">◦ Developed with the software and tools below.</h3>
<p align="center">
  <img src="https://img.shields.io/badge/Language-Python-blue" alt="">
  <img src="https://img.shields.io/badge/Framework-discord.py-red" alt="">
  <img src="https://img.shields.io/badge/Database-PostgreSQL-blue" alt="">
</p>
<p align="center">
  <img src="https://img.shields.io/github/badge/license-MIT?style=flat-square&color=5D6D7E" alt="GitHub license" />
  <img src="https://img.shields.io/github/last-commit/spectra-ai-codegen/Discord-Mini-Games-Bot?style=flat-square&color=5D6D7E" alt="git-last-commit" />
  <img src="https://img.shields.io/github/commit-activity/m/spectra-ai-codegen/Discord-Mini-Games-Bot?style=flat-square&color=5D6D7E" alt="GitHub commit activity" />
  <img src="https://img.shields.io/github/languages/top/spectra-ai-codegen/Discord-Mini-Games-Bot?style=flat-square&color=5D6D7E" alt="GitHub top language" />
</p>

## 📑 Table of Contents
- [📍 Overview](#overview)
- [📦 Features](#features)
- [📂 Repository Structure](#repository-structure)
- [💻 Installation](#installation)
- [🏗️ Usage](#usage)
- [🌐 Hosting](#hosting)
- [📄 License](#license)
- [👏 Authors and Acknowledgments](#authors-and-acknowledgments)

## 📍 Overview
This project aims to develop a Discord bot that enables users to play fun and engaging mini PvP games directly within their Discord server. The bot will provide a seamless and interactive experience, enhancing server community engagement and adding an exciting element of competition.

## 📦 Features
- **Discord Integration:** The bot will seamlessly integrate with Discord using the Discord API.
- **Game Selection:** Users can choose from a variety of mini-games like Tic-Tac-Toe, Rock Paper Scissors, and Trivia.
- **Matchmaking:** The bot facilitates matchmaking based on game type and user preferences.
- **In-Game Mechanics:**  Players interact with the bot using Discord commands to make moves, answer questions, or take actions within the game.
- **Leaderboards:** Leaderboards track player progress and rankings for each game.
- **Customization:** Server administrators can customize settings such as enabling/disabling games, setting designated game channels, and defining command prefixes.
- **User Interface:** A user-friendly interface will guide users through game selection, matchmaking, gameplay, and accessing information.

## 📂 Repository Structure

```
├── bot
│   ├── cogs
│   │   ├── games
│   │   │   ├── rock_paper_scissors.py
│   │   │   ├── tic_tac_toe.py
│   │   │   └── trivia.py
│   │   ├── admin.py
│   │   └── general.py
│   ├── database
│   │   ├── models.py
│   │   └── db_utils.py
│   ├── utils
│   │   ├── embeds.py
│   │   ├── matchmaking.py
│   │   └── game_logic.py
│   └── main.py
├── requirements.txt
└── .env

```

## 💻 Installation
### 🔧 Prerequisites
- Python 3.8 or higher
- pip (package installer for Python)
- PostgreSQL (for database)

### 🚀 Setup Instructions
1. **Clone the repository:**
   ```bash
   git clone https://github.com/spectra-ai-codegen/Discord-Mini-Games-Bot.git
   ```
2. **Navigate to the project directory:**
   ```bash
   cd Discord-Mini-Games-Bot
   ```
3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
4. **Set up environment variables:**
   - Create a `.env` file (if it doesn't exist) and add the following:
     ```
     DISCORD_TOKEN=YOUR_DISCORD_BOT_TOKEN
     DATABASE_URL=postgresql://USER:PASSWORD@HOST:PORT/DATABASE
     PREFIX=! 
     ```
   - Replace placeholders with your actual values:
     - `DISCORD_TOKEN`:  Your Discord bot token.
     - `DATABASE_URL`:  Your PostgreSQL database connection string.
     - `PREFIX`:  The default command prefix for the bot (optional, default is `!`).

## 🏗️ Usage
### 🏃‍♂️ Running the Bot
1. **Start the bot:**
   ```bash
   python bot/main.py
   ```
2. **Invite the bot to your Discord server:**
   - Go to [https://discord.com/api/oauth2/authorize?client_id=YOUR_BOT_CLIENT_ID&permissions=8&scope=bot](https://discord.com/api/oauth2/authorize?client_id=YOUR_BOT_CLIENT_ID&permissions=8&scope=bot) (Replace `YOUR_BOT_CLIENT_ID` with your bot's Client ID).

## 🌐 Hosting
### 🚀 Deployment Instructions
1. **Dockerize the project:**
   - Create a `Dockerfile` in the project root:
     ```dockerfile
     FROM python:3.8-slim
     WORKDIR /app
     COPY requirements.txt .
     RUN pip install -r requirements.txt
     COPY . .
     CMD ["python", "bot/main.py"]
     ```
2. **Build the Docker image:**
   ```bash
   docker build -t discord-mini-games-bot .
   ```
3. **Run the Docker container:**
   ```bash
   docker run -d -p 80:80 discord-mini-games-bot
   ```
4. **Host the container on a cloud platform:**
   - You can use services like Heroku, AWS, Google Cloud, etc. to host the Docker container.

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors and Acknowledgments
- **Author Name** - [Spectra.codes](https://spectra.codes)
- **Creator Name** - [DRIX10](https://github.com/Drix10)

<p align="center">
    <h1 align="center">🌐 Spectra.Codes</h1>
  </p>
  <p align="center">
    <em>Why only generate Code? When you can generate the whole Repository!</em>
  </p>
  <p align="center">
	<img src="https://img.shields.io/badge/Developer-Drix10-red" alt="">
	<img src="https://img.shields.io/badge/Website-Spectra.codes-blue" alt="">
	<img src="https://img.shields.io/badge/Backed_by-Google_&_Microsoft_for_Startups-red" alt="">
	<img src="https://img.shields.io/badge/Finalist-Backdrop_Build_v4-black" alt="">
  <p>