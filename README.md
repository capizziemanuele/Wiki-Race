<p align="center">
  <img src="docs/banner.png" alt="Wiki Race: race through Wikipedia, one link at a time" width="100%">
</p>

<p align="center">
  <a href="https://YOUR-USERNAME.github.io/wiki-race/"><img src="https://img.shields.io/badge/%E2%96%B6%20Play%20now-free%20in%20your%20browser-b4441c?style=for-the-badge" alt="Play now, free in your browser"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/works%20on-phone%20%C2%B7%20tablet%20%C2%B7%20desktop-1d2321" alt="Works on phone, tablet and desktop">
  <img src="https://img.shields.io/badge/multiplayer-live%20rooms-1f7a4d" alt="Live multiplayer rooms">
  <img src="https://img.shields.io/badge/sign--up-not%20needed-5f6964" alt="No sign-up needed">
  <img src="https://img.shields.io/badge/license-MIT-2a5db0" alt="MIT license">
  <a href="https://buymeacoffee.com/beele"><img src="https://img.shields.io/badge/Buy%20me%20a%20coffee-FFDD00?logo=buymeacoffee&logoColor=black" alt="Buy me a coffee"></a>
</p>

# Wiki Race

**Wiki Race is a free Wikipedia game you play in your browser.** You start on one Wikipedia article and try to reach another one using only the links inside the page. The fewer clicks, the better. You may know it as the Wikipedia game, wikiracing or six degrees of Wikipedia.

Play on your own, take the daily race, or open a room and race your friends live from your phones.

<p align="center">
  <img src="docs/screenshot-home.png" alt="Home screen with a silly pair from Pizza to Black hole, the daily race and multiplayer" width="66%">
  &nbsp;
  <img src="docs/screenshot-multiplayer-phone.png" alt="Multiplayer results on a phone, with a podium and the round's scores" width="26%">
</p>

## How to play

1. **Look at the target.** The target card shows a short summary, its categories and the topics its introduction mentions.
2. **Click links inside the article.** Links in text, lists, tables and infoboxes all count. Portals, categories and files don't.
3. **Reach the target.** Going back is allowed but costs a click, and so does a hint.

When the target is linked on the page you're reading, the link turns green.

<p align="center">
  <img src="docs/screenshot-race.png" alt="A race in progress, with the Hot and cold thermometer, the target card and the hint button" width="92%">
</p>

## Features

- **Pick a pair your way.** Random articles, 12 themed categories (Food & drink, Animals, Space, Myths & legends, Weird & wonderful and more), what people are reading on Wikipedia today, or your own words.
- **Make your own categories.** Build one from a list of articles or from any Wikipedia category, then share it with a link.
- **Trivia trails.** 28 ready-made routes that end with a true and surprising fact. Did you know bubble wrap was invented as a wallpaper?
- **Silly pairs.** From Kevin Bacon to Bacon, from a rubber duck to the Titanic, and 15 more.
- **Three modes.** Classic (fewest clicks), Time attack (beat the clock) and Six degrees (six clicks, not one more).
- **Six twists you can stack.** See the table below.
- **Daily race.** The same pair for everyone each day, with a streak and a result you can share.
- **Live multiplayer.** Rooms with a 5-letter code, an invite link or a QR code, a live scoreboard, emoji reactions and points across rounds.
- **Challenge links.** Send your result to a friend and see if they can beat it. No server needed.
- **Fun extras.** 23 achievements, stats, hints, a shortest-route check after each race, article previews on hover, find on page, sounds and a dark mode.
- **10 Wikipedias.** English, Simple English, Italian, French, German, Spanish, Portuguese, Dutch, Polish and Swedish.

<p align="center">
  <img src="docs/screenshot-modes.png" alt="Category picker, modes and twists" width="92%">
</p>

## Twists

| Twist | What it does |
|---|---|
| 🙈 Mystery target | The target's title is hidden. You only get clues. |
| 🚫 No going back | The back button is gone. Commit to every click. |
| 👻 Invisible links | Links look like plain text. |
| 🌡️ Hot & cold | A thermometer tells you if you're getting closer. |
| 🌀 Chaos | Random events: teleports, mirror world, Comic Sans, banana peels. |
| 🚧 No shortcuts | Big hub pages like countries and world wars are blocked. |

## Multiplayer

Click **Create a room** and share the code, the invite link or the QR code. Everyone races the same pair at the same time, and the board shows who's ahead. The host picks the pair, the mode and the twists. If the host leaves, someone else takes over.

Rooms pass their messages through free public MQTT servers, so there's nothing to set up. These are shared test servers, though, and some school or office networks block them. If that happens, send a challenge link instead, or enter your own MQTT WebSocket server in **Settings**.

## Keyboard shortcuts

| Key | Action |
|---|---|
| `/` | Find a link on the page |
| `B` | Go back |
| `H` | Hint |
| `T` | Show the target (phone layout) |
| `Esc` | Close panels |

## Run your own copy

The whole game is a single `index.html` file. There's no build step and nothing to install.

1. Fork this repository.
2. Open **Settings → Pages**, choose **Deploy from a branch**, then branch `main` and folder `/ (root)`.
3. After a minute or two, your copy is live at `https://<your-username>.github.io/wiki-race/`.

You can also open `index.html` straight from your computer, or put it on any host that serves static files.

The **Buy me a coffee** button links to my page. To change or remove it in your copy, search `index.html` for `SUPPORT_URL` and put in your own link, or an empty string. The button also hides itself when the game runs inside another website, such as a game portal, or inside an Android app that opens it with `?app=android`.

## Privacy

There are no accounts, no cookies, no ads and no analytics. Your stats, achievements and categories stay in your browser's local storage. Articles load directly from Wikipedia's public API, and fonts load from Google Fonts. When you open a room, the multiplayer and QR code libraries load from jsDelivr, and your chosen name, avatar and race progress are shared with the other players through the room's message server.

## Support

Wiki Race is free and has no ads. If it gave you a good laugh or taught you something odd, you can buy me a coffee. Thank you!

<a href="https://buymeacoffee.com/beele"><img src="https://img.shields.io/badge/%E2%98%95%20Buy%20me%20a%20coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black" alt="Buy me a coffee"></a>

## Contributing

Ideas, bug reports and new trivia trails are welcome. Please open an issue.

## Credits

- Article text and images come from [Wikipedia](https://www.wikipedia.org/) and Wikimedia Commons under their own licences, mostly [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Every article in the game links back to its source.
- Wiki Race is a fan project. It isn't affiliated with or endorsed by Wikipedia or the Wikimedia Foundation.
- Multiplayer uses [MQTT.js](https://github.com/mqttjs/MQTT.js), and invite QR codes use [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator). Both are MIT licensed.
- Fonts: Fraunces, Source Serif 4 and IBM Plex Mono from Google Fonts, under the SIL Open Font License.

## License

The game's code is released under the [MIT License](LICENSE). Wikipedia content keeps its own licence.
