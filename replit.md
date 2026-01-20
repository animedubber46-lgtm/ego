# Video Encoder Bot

## Overview
A Telegram bot for encoding/converting videos with various features including direct link downloading, Google Drive integration, and queue management.

## Project Structure
- `VideoEncoder/` - Main bot package
  - `__init__.py` - Bot initialization and configuration
  - `__main__.py` - Entry point
  - `plugins/` - Bot command handlers (auth, encode, upload, etc.)
  - `utils/` - Utility functions (encoding, helpers, settings)
  - `video_utils/` - Video processing utilities
- `config.env` - Environment configuration file

## Configuration
The bot requires the following environment variables in `config.env`:
- `API_ID` - Telegram API ID
- `API_HASH` - Telegram API Hash
- `BOT_TOKEN` - Telegram Bot Token (from @BotFather)
- `OWNER_ID` - Bot owner's Telegram ID
- `SUDO_USERS` - Space-separated list of sudo user IDs
- `EVERYONE_CHATS` - Space-separated list of chat IDs
- `LOG_CHANNEL` - Log channel ID
- `MONGO_URI` - MongoDB connection URI
- `SESSION_NAME` - Session name for the bot

## Dependencies
- Python 3.10
- pyrofork (Pyrogram fork)
- ffmpeg (system)
- mediainfo (system)
- MongoDB

## Running
The bot runs as a worker process:
```bash
python3 -m VideoEncoder
```

## Recent Changes
- January 2026: Initial setup in Replit environment
