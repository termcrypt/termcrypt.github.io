---
layout: default
title: Market Commands
parent: Commands
permalink: /commands/market-info
---

## Market Commands
These are the available market-based commands that termcrypt has currently.

### price | p
Get the latest prices of the current market.

### search [query]
Search all market pairs for your query. An example is searching for `bat` and it will return all pairs beginning with or ending with `BAT`. You can also search here for pairs, so if you want to search for a future format the search like this: `coin-perp/1231` otherwise, for spot, search like this: `coin/coin`.

### pair
Change termcrypt's current pair to your input. This command automatically detects if the pair is a future and checks for it with the future formatting (`-`) rather than the spot formatting (`/`). This command does not support multiple dash markets like: `BTC-MOVE-2022Q1`.

### orderbook | ob
Get a display of the current orderbook. It shows both bids and asks for the current pair with a depth of 10.