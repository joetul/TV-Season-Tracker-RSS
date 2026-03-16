
# SeasonFeed

Never miss a new TV season. Subscribe to RSS feeds for your favorite shows and get notified when a new season is announced.

**Live site:** [joetul.github.io/SeasonFeed](https://joetul.github.io/SeasonFeed/)

## How It Works

1. Browse the show list on the site.
2. Click **Copy RSS** to grab a feed URL.
3. Paste it into your RSS reader (FeedFlow, NetNewsWire, etc.).

You can also select multiple shows and export them as an OPML file for bulk import.

Feeds are generated daily using data from the [TVmaze API](https://www.tvmaze.com/api).

## Show Missing?

SeasonFeed is a community-maintained list. We can't simply add every show on TVmaze — only shows that are manually added and reviewed are included. This keeps the list focused and the feeds reliable.

If a show you want isn't listed, you can help grow the list:

- **[Open an issue](https://github.com/joetul/SeasonFeed/issues/new?labels=show-request&title=Request%3A+Add+[SHOW+NAME])** — include the show title and a TVmaze link if possible.
- **[Submit a PR](https://github.com/joetul/SeasonFeed/pulls)** — add the show to `shows.json` and open a pull request.

Shows can be added by name or with an explicit TVmaze ID:

```json
{
  "shows": [
    "Severance",
    { "name": "Andor", "tvmaze_id": 33073 }
  ]
}
```

## License

MIT
