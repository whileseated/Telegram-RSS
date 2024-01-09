# Telegram RSS Bot

A straightforward, database-free RSS reader bot for Telegram, designed for easy tracking of your favorite RSS feeds directly through Telegram messages.

## Features

- **No Database Required**: Uses a simple text file (`feeds.txt`) for managing subscriptions.
- **Easy Configuration**: Just a `config.txt` file for Telegram Token and Chat ID.
- **Supports Common RSS Formats**: Compatible with most RSS/Atom feeds.
- **User-Friendly Commands**: Add, check, and remove feeds with intuitive Telegram bot commands.

## Setup

### Prerequisites

- Python 3.x
- `python-telegram-bot` module (version 13.7)
- `feedparser` module

### Installation

1. **Create a Telegram Bot**:
   - Use [@BotFather](https://t.me/botfather) to create a new Telegram bot. This will generate your Telegram Token.
   - Find your personal chat ID using [@userinfobot](https://t.me/userinfobot).

2. **Configuration File**:
   - Create a `config.txt` file.
   - Add your Telegram Token and your Chat ID on separate lines:

     ```
     your_telegram_token
     your_telegram_chat_id
     ```

3. **Feeds File**:
   - Create a blank `feeds.txt` file for your RSS subscriptions.
   - When the bot adds a subscription (one per line), the feed information is formatted as follows: `RSS URL | NICKNAME | LAST POST URL`

4. **Install Dependencies**:
   Run the following commands to install necessary Python modules:

```
pip install python-telegram-bot==13.7
pip install feedparser
```

### Running the Bot

Execute the script to start the bot:

```
python3 telegram_rss.py

```

Keep the script running to maintain the bot's functionality.

## Usage

Interact with the bot using these commands:

- **Add a Feed**: Simply paste an RSS/Atom feed URL into the chat.
- **Check Feeds**: Type `check` to review the latest posts from all subscribed feeds.
- **Remove a Feed**: Use `remove` and follow the UI picker to unsubscribe from a feed.

### Customizing Bot Commands

Configure additional bot commands through [@BotFather](https://t.me/botfather) to make them available in the bot's menu.

## Planned Features

- [ ] Automatic feed checks every 15 minutes.
- [ ] Start message for new users.
- [ ] Cancel option for each command.
- [ ] Command to display all subscribed feeds.
- [ ] Dockerize it all.

## Demonstration

![Telegram RSS Bot in Action](telegram_rss.GIF)
