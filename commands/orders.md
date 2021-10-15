---
layout: default
title: Order-Based Commands
parent: Commands
permalink: /commands/orders
---

## Order-Based Commands
Termcrypt has many different market info commands that get data from exchange apis and then display the info to the user.

When making queries, there is a slight delay, and that is the REST request to the exchange API.

### lev
Get current account leverage. This is the same across all subaccounts.

### lev [number]
Change leverage to chosen number. FTX supports 1-5, 10, 20, 50 & 100.

### order | o
This command initiates an order. An order inside of termcrypt is the beginning of a trade. A trade in termcrypt consists of an entry, stoploss, and take-profit which are all combined together to create the whole trade. If you want to learn more about orders, visit the orders category.