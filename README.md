**Telegram RSS Bot**

1. Create a config.txt file with your Telegram Token and Chat ID, each on one line

```
telegram token
telegram chat id
```

2. feeds.txt contains your subscriptions, one-per-line. Each line is comma separated in three segments, containing this info: RSS URL | NICKNAME | LAST POST URL
3. telegram_rss.py is the script. It's been built (and tested) with python-telegram-bot module (13.7 version). To install:

```
pip install python-telegram-bot=13.7
pip install feedparser
```

4. Run the script

```
python3 telegram_rss.py
```

The commands available in the script are:
- add a feed (paste a rss/atom feed into the tool without typing add)
- "check" (checks all feeds for latest post)
- "remove" (unsubscribe from a feed in feeds.txt with a UI picker)

![test](https://imgur.com/a/fotalaT)
![alt text](telegram_rss.GIF)
