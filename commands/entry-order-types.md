---
layout: default
title: Entry Order Types
parent: Commands
permalink: /commands/entry-order-types
---

## Entry Order Types
The entry order types are what you choose when opening an order. For entry order types, all are capable of opening a long and short order while in future pairs.

For more information on fees (for ftx), visit [this article](https://help.ftx.com/hc/en-us/articles/360024479432-Fees).

### default (limit/stop)
This is the default order type, for when you enter in a price when you open an order. This type uses a single limit/stop order with post-only enabled.

You should use this order type if you want to enter a position but the price is not at the entry area yet. If you want to enter an order now, it is advised to enter with the orderbook order type.

### m (market)
This order type opens a market order to open an almost guaranteed-fill order for the latest price.

### ob (orderbook)
The order book entry type opens a limit order with your specified orderbook position. If the order crosses the book, it will retry the order up to 10 times. The order has post-only enabled to make sure you get the right fees.