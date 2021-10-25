---
layout: page
title: Getting Started
permalink: /getting-started/
has_children: false #change
---

## Getting started

This section is a comprehensive introduction for new users who have no experience with termcrypt. Termcrypt is made to be run in a terminal emulator. We recommend [alacritty](https://alacritty.org/) for linux, mac and windows. We also recommend [termux](https://termux.com/) for android and [newterm](https://github.com/hbang/NewTerm) for ios (untested).

You should follow the installation steps on our repository. Then after that, you should type and enter `termcrypt` in a terminal.

If it says command not found / file not found, that means you did not install it correctly. Either your PATH is not set or termcrypt was never installed. Follow the installation steps from the beginning. If you recieve any other error on launch, report it in our github issues section.

The first thing you will have to do is enter the API keys for your exchange. The public key may be called API key on its own (on the exchange) and the private key may be called API secret. Do not share these API keys with anyone, especially the private key.

### Basic controls

Before getting started with commands, you should know the most basic controls for termcrypt. UP and DOWN arrow keys will change the input to your history (means you can input last command). Pressing `CTRL` and `c` at the same time will close termcrypt. Pressing `q` then `enter` when in a parameter input will exit the command.

### Basic commands

you can use `help` or `h` to get a list of the available commands for termcrypt.