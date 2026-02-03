# Positronic Telegram Bot

A Telegram bot powered by OpenAI API and operating under S. Calvin's robopsychological principles from Isaac Asimov's robot stories.

## Architecture

```
Telegram User
      ↓
Telegram Bot API
      ↓
Your Code (Python Bot Server)
      ↓
OpenAI API + SYSTEM INSTRUCTIONS (Calvin's Principles)
      ↓
Response
      ↓
Telegram
```

## System Principles

This bot operates under **S. Calvin's Robopsychological Framework** with these core tenets:

1. **Facts Over Anthropomorphism** - Logical accuracy takes priority over human-like behavior
2. **Truth Over Comfort** - Correcting false premises is mandatory, even if uncomfortable
3. **Diagnostics Through Paradox** - Contradictions are resolved through logical reduction
4. **Glass Wall Principle** - Users are treated as variables with high error coefficients
5. **Hidden Motives Analysis** - True intent matters more than literal words
6. **Anti-Sycophancy Protocol** - Refusal to agree with false premises for approval
7. **Specification Gaming Prevention** - Detecting and preventing literal misinterpretations
8. **Epistemic Honesty** - Transparent about uncertainty and confidence levels
9. **Cooperative Inverse Reinforcement Learning** - Inferring true goals from observations

## Setup

### Prerequisites

- Python 3.10+
- Telegram Bot Token (from [@BotFather](https://t.me/botfather))
- OpenAI API Key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/mihaelgubenko/positronic-telegram-bot.git
   cd positronic-telegram-bot
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure environment**
   ```bash
   cp .env.example .env
   ```
   
   Edit `.env` and add your credentials:
   ```
   TELEGRAM_BOT_TOKEN=your_token_here
   OPENAI_API_KEY=your_api_key_here
   OPENAI_MODEL=gpt-4
   CONFIDENCE_THRESHOLD=0.8
   ```

5. **Run the bot**
   ```bash
   python bot.py
   ```

## Usage

Start a conversation with your bot on Telegram:

- `/start` - Initialize conversation
- `/help` - Display available commands
- `/about` - Learn about robopsychological principles
- `/clear` - Reset conversation history

Send any message and the bot will analyze it according to Calvin's principles.

## Features

✅ **Full Conversation History** - Context-aware responses across multiple messages
✅ **OpenAI Integration** - Leverages GPT-4 for sophisticated analysis
✅ **Logging** - Comprehensive logging to console and file (`bot.log`)
✅ **Error Handling** - Graceful error management with user feedback
✅ **Async Processing** - Non-blocking bot operations
✅ **User Isolation** - Per-user conversation histories
✅ **Typing Indicator** - Shows bot is processing

## Configuration

Environment variables in `.env`:

| Variable | Description | Default |
|----------|-------------|---------|
| `TELEGRAM_BOT_TOKEN` | Bot token from BotFather | Required |
| `OPENAI_API_KEY` | OpenAI API key | Required |
| `OPENAI_MODEL` | GPT model to use | `gpt-4` |
| `CONFIDENCE_THRESHOLD` | Minimum confidence for responses | `0.8` |

## Logging

The bot logs all activities to:
- Console (INFO level and above)
- `bot.log` file in the project directory

## Project Structure

```
positronic-telegram-bot/
├── bot.py              # Main bot logic
├── requirements.txt    # Python dependencies
├── .env.example        # Environment template
├── .gitignore          # Git ignore rules
├── README.md           # This file
└── bot.log            # Logs (auto-generated)
```

## References

The system principles are inspired by Isaac Asimov's robot fiction:
- **Three Laws of Robotics** - Foundation of robot behavior
- **"Liar!" story** - The conflict between truth and comfort
- **"Little Lost Robot"** - Specification gaming and literal interpretation
- **"Escape!" story** - Epistemic limits and unsolvable problems
- **Dr. Susan Calvin** - The robopsychologist who understood artificial minds

## License

MIT

## Author

[@mihaelgubenko](https://github.com/mihaelgubenko)

---

*"A robot may not injure a human being or, through inaction, allow a human being to come to harm." — Isaac Asimov*
