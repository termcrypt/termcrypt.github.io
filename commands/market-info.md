---
layout: default
title: Market Information
parent: Commands
permalink: /commands/market-info
---

## Market Information Commands
Termcrypt has many different market info commands that get data from exchange apis and then display the info to the user.

When making queries, there is a slight delay, and that is the REST request to the exchange API.

### price | p
Get the latest prices of the current market.

### search [query]
Search all market pairs for your query. An example is searching for `bat` and it will return all pairs beginning with or ending with `BAT`. You can also search here for pairs, so if you want to search for a future format the search like this: `coin-perp/1231` otherwise, for spot, search like this: `coin/coin`.

### pair
Change termcrypt's current pair to your input. This command automatically detects if the pair is a future and checks for it with the future formatting (`-`) rather than the spot formatting (`/`). This command does not support multiple dash markets like: `BTC-MOVE-2022Q1`.