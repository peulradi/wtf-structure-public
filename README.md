# Nexus Bot — A Monument to Spaghetti Code

> 23,000+ lines. One Python file. Zero classes. No regrets.

This project is an intentionally over-engineered, under-architected Discord bot built almost entirely inside a single Python file.

It is not an accident.

It is not waiting to be refactored.

It is not a cry for help.

This is an art piece expressing my profound contempt for structural organization through executable Python.

## The Philosophy

Modern software engineering tells us to:

* separate concerns
* use meaningful names
* split large modules
* encapsulate state
* design clean abstractions
* write maintainable code

I considered these suggestions carefully.

Then I put **23,000+ lines into one file**.

The goal of this project is simple:

> How wrong can software architecture become while the software itself remains functional?

This repository is my attempt to answer that question.

## ✨ Features

Despite its architectural crimes, it actually works.

Inside this single file lives a Discord bot containing hundreds of commands and features including:

* moderation and administration
* security and anti-raid systems
* AI-powered features
* music playback
* TTS
* translation
* logging and statistics
* verification systems
* economy and minigames
* blackjack
* a text RPG
* stock, cryptocurrency, and exchange-rate tools
* server management utilities
* and various other things that probably deserved their own modules

They did not receive their own modules.

## 🏗️ Architecture

There isn't one.

```text
bot.py
└── everything
```

No `services/`.

No `models/`.

No `utils/`.

No `cogs/`.

No `src/`.

Just Python.

A lot of Python.

## 📊 Technical Achievements

* 23,000+ lines of Python
* 1 source file
* 0 classes
* 800+ functions
* 300+ Discord commands
* an unreasonable number of dictionaries
* function names that provide approximately zero emotional support
* somehow still executable

Some people use classes.

I use `dict`.

Some people use modules.

I use scrolling.

Some people use dependency injection.

I use faith.

## ⚠️ Is this good code?

No.

Is it functional software?

Surprisingly, yes.

That distinction is the entire point.

This project intentionally sacrifices readability, modularity, discoverability, and maintainability while attempting to preserve actual functionality.

Bad code is easy to write.

Writing bad code that still works at 23,000 lines requires commitment.

## 🔧 Contributing

Before submitting a pull request, ask yourself:

> “Does this make the architecture cleaner?”

If yes, please reconsider.

Refactoring may constitute vandalism of the artwork.

Bug fixes are welcome.

Architectural improvements are viewed with suspicion.

## 🖼️ Artistic Statement

This repository should not be interpreted merely as poorly structured software.

It is an executable monument to the rejection of unnecessary order.

Every numbered function is a brushstroke.

Every global dictionary is a rejection of hierarchy.

Every additional thousand lines in `bot.py` brings us further from clean architecture and closer to truth.

The code is the documentation.

Unfortunately, the code is 23,000 lines long.

## License

Use it, study it, laugh at it, question it.

Just don't split the file.

## Local setup

Requires Python 3.10 or newer. Keep the intentionally single-file structure.

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
Copy-Item .env.example .env
# Fill .env locally, then start when ready:
.\.venv\Scripts\python.exe bot_final_REAL_do_not_refactor.py --no-gui
```

Set `DISCORD_TOKEN`, `OPENAI_API_KEY`, and comma-separated `BOT_ADMIN_IDS` in the local `.env`. SMTP settings and `PURGE_PASSWORD` are optional. Enable the Message Content and Server Members privileged intents in the Discord developer portal. GUI mode is the default when `--no-gui` is omitted and requires Tkinter. Music playback may require FFmpeg installed separately. The bot creates local state, user records, message/action logs, and a SQLite database; keep these private and out of Git.
