# Four in a Row

Drop discs, block your friend, line up four. A multiplayer starter game from [Multiplayer Agent](https://multiplayeragent.com): 2D, turn-based, 2 players plus anyone who wants to watch, with a bot that takes any empty seat.

![Four in a Row](poster.jpg)

## How it plays

Take turns dropping a disc into one of seven columns; the first to get four in a line across, down or diagonally wins. The first two players take the seats; anyone else watches and takes the loser's seat next game. Alone? A bot plays the other side, and a friend who joins takes over from it. Two players get 45 seconds a drop, then one is made for them.

**Controls:** Click or tap a column (or press 1–7) to drop a disc.

## Make it yours in the Game Builder

Open the [Game Builder](https://multiplayeragent.com), choose **Start from a starter game** and pick Four in a Row. It opens as version 1 in your studio, ready to play and publish. Then ask for changes, for example:

- Make the board 9 wide and 5 to win
- Add a 15-second timer for each turn
- Turn the discs into cookies and the board into an oven tray

## Run it yourself

1. Get a free publishable key (`pk_…`) at [multiplayeragent.com](https://multiplayeragent.com).
2. In `index.html`, put it in place of `pk_REPLACE_ME` in the `MP_CONNECT` block.
3. Open `index.html` in a browser. No build step and no server needed.

Without a key it still runs, offline against the bot.

## How it is built

- One `index.html`. The comment at the top of the script maps the code and explains the multiplayer.
- **Host-run rules:** The host's browser checks every drop; if it leaves, the next player takes over.
- **Bots:** A bot takes any empty seat, so you can play alone, and a friend who joins takes the bot's side.
- **Live sync:** Players and watchers see the same board, and you see your opponent's disc hover before it drops.
- **Leaderboard:** Most wins, shown after every game.
- `?attract` runs it offline, bot against bot. The preview video is recorded from it.

## License

MIT.
