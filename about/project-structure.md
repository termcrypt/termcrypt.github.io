---
layout: default
title: Project Structure
parent: About
permalink: /about/project-structure
---

## Project Structure

The project structure is one of a typical rust application. The code is contained in `src` and once built, the executables are contained in `target`.

The highest level inside of termcrypt contains a few files. `.gitignore` is a hidden file that stops unwanted files from being uploaded to the repository when pushed. `Cargo.lock` contains all the information for the rust crates used in the project (normally you do not edit this file). `Cargo.toml` contains the project information, and the explicit imports for custom crates. `rustfmt.tml` contains the formatting configuration used when `cargo fmt` is ran.

Inside of `src`, the project starts at `main.rs`. It initializes several project variables and also checks the database using functions from `db.rs` for configuration and api keys. After that, it starts a loop where is asks for the user input. After the user inputs text, it is given into `ftx_exchange/ftx_inter.rs` and `misc.rs`. Inside these modules, they both use the function `handle_commands` to process and match the user text. If it matches the comparison arms in these files, then the code in the arms will be executed. If an error comes from the command handling, then it will not cause the application to panic, unless it is explicitly told to, with `.unwrap()` or similar. After that, the loop starts again, adding the user input to the history if it is a valid command.

### utils
This module contains utility functions that are unanimously used accross different exchanges. Exchange-specific utilities are contained inside of their specific subfolder.

### db
This module is used for interacting with the database. Termcrypt currently uses `sled` for a database module, and it stores the information in the operating system's `data_dir` directory, which on linux, is stored in `~/.local/share/termcrypt/db`.

### ftx_exchange/

Inside of this folder, it has a file called `mod.rs` which sources and uses all of the modules in the folder. This allows `main.rs` and other higher components to use the functions inside of the folder. `ftx_advanced_orders.rs` is used to process and execute orders. `ftx_inter.rs` handles commands as said previously. `ftx_utils` contains utility functions that are specific to the FTX exchange.