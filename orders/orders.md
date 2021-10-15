---
layout: page
title: Orders
permalink: /orders/
has_children: true
---

## Orders
This section contains all relevant information for making orders in termcrypt.

All of the sections below talk about what happens after the order command is initiated.

### Notes before you open a trade
It is advised to change your leverage if you want to have more liquidity for other trades, or if you need more of assets to borrow.

### Risk
Risk management is a large part of termcrypt's purpose and orders have been designed to be dynamically sized based on your risk %. The risk % defines the percentage of the current subaccount you want to lose if the stoploss for the trade is hit. If you want to lose 1.5% of your subaccount if your stoploss is hit then you can enter `1.5` for the risk parameter.

### Stoploss
The stoploss defines the price to where you want the main order to exit if it goes the wrong direction. The stoploss type is defined later.

### Take-Profit
The tp defines the price where you want the main order to exit if it succeeds. Similar to the stoploss, the type is defined later.

### Entry
The entry is a more complicated parameter. The entry parameter accepts either types, or a number to open a trigger limit/stop limit order. If I wanted to execute an order to buy BTC if it hit 31030$, I would enter: `31030`. If I wanted to enter using the `ob` type, I would enter: `ob`. More information on entry types is in the Entry Order Types page in the current section.

### Confirmation
Look over the parameters and confirm that they are okay. Because termcrypt is in early development, is it better to be sure about the order quantity.

#### Order Size
This field shows the order size that the trade will have, calculated from your risk %.

#### SL-TP Ratio
This field will show you the ratio between the entry and stoploss, compared to the entry and take-profit. This is useful for knowing if trades are favourable / if you want to proceed with them on second thought.

#### % Of Sub Liquidity
This field shows you the percentage of the subaccount that will be used if the trade proceeds.

#### Entry Fees
This field gives you the predicted fees in terms of the asset and subaccount balance for your chosen ordertype. This does not include order exit fees however.

### Stoploss Type
After the order has completed, you will be given the inputs to enter the stoploss type and take-profit types that you want. You can find more about the available stoploss types on the Stoploss Order Types page in the current section.

### Take-Profit Type
This is a similar parameter as above, but with potentially differing types, so check out the Take-Profit Order Types page in the current section.

## Fini!
After all of this the trade should be complete.

If you had any problems with opening a trade, please open an issue on our repository.