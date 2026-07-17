# ticket-giveaway-data

The published giveaway list for the **Ticket Giveaway Tracker** app. The app fetches
`contests.json` from this repo's raw URL when you tap "Check for updates".

Raw URL (baked into the app):
https://raw.githubusercontent.com/ericvisser/ticket-giveaway-data/main/contests.json

## Updating

1. In the app project, edit `electron/default-contests.json` (add artists/giveaways,
   bump the `"version"` to today's date) and run `npm run validate`.
2. Run `npm run publish-data` in the app project — it copies the list here.
3. `git add contests.json && git commit -m "Update <version>" && git push`

Everyone's app picks up the new list on their next "Check for updates".
