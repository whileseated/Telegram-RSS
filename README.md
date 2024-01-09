*Telegram RSS Bot*
---

A super simple, databaseless RSS reader for Telegram.

**This python script keeps track of your subscriptions using a plain text file, feeds.txt. You'll need to find your Telegram Token and target CHAT ID, and include those values in config.txt**

1. Use the BotFather to create your own Telegram bot/channel, which will generate your Telegram Token. You can use @userinfobot to find your own, personal chat ID. 

2. Create a config.txt file with your Telegram Token and your Chat ID, each on one line, like this:

```
telegram_token
your_telegram_chat_id
```

3. feeds.txt contains your subscriptions, one-per-line. Each line is comma separated in three segments, containing this info: RSS URL | NICKNAME | LAST POST URL
4. telegram_rss.py is the script. It's been built (and tested) with python-telegram-bot module (13.7 version). To install:

```
pip install python-telegram-bot=13.7
pip install feedparser
```

5. Run the script, and keep it running.

```
python3 telegram_rss.py
```

Using @botfather you can configure commands so they're available in the bot's menu. The commands available in the script are:
- add a feed (paste a rss/atom feed directly into the tool, no need to preface with "add")
- "check" (checks all feeds for latest post)
- "remove" (unsubscribe from a feed in feeds.txt with a UI picker)

![alt text](telegram_rss.GIF)

To Do:
- Have script "check" feeds on its own every 15 minutes
- Need message for when /start occurs 
- Create a "cancel" option for each command
- Need a "show all feeds" command