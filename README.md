**Telegram RSS Bot**

1. Create a config.txt file with your Telegram Token and Chat ID, each on one line

```
telegram token
telegram chat id
```

2. feeds.txt contains your subscriptions, one-per-line. Each line is comma separated, like this: RSS URL | NICKNAME | LAST POST URL
3. telegram_rss.py is the script. It's been built (and tested) with python-telegram-bot module (13.7 version). To install:

```
pip install python-telegram-bot=13.7
pip install feedparser
```

more stuff here


![test](https://imgur.com/a/fotalaT)