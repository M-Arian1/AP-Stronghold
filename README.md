# Stronghold: a medieval strategy game in Java

A team remake of the strategy game *Stronghold Crusader*, built for the Advanced Programming course at Sharif University of Technology (spring 2023). Java 17, JavaFX, Gson persistence and JUnit tests, in an MVC structure with a client–server online mode.

**Team 48:** Parsa Ghezelbash, Farnam Forghani, Arian Tehrani.

## What it does
- **Accounts:** sign up and log in with a captcha, password recovery, profiles with avatars, and a scoreboard.
- **Maps:** tile maps with land textures you can set per cell, saved and loaded between sessions.
- **Your castle:** place buildings (gatehouses, towers, storage, inns, industrial and recruitment centres, traps), manage resources and keep your popularity up through food, tax, religion and fear.
- **People and war:** recruit workers and troops of different nations, move them across the map and fight, with walking and fire animations.
- **Economy:** a shop for buying and selling resources, and trade requests between players with a trade history.
- **Matches:** turn-based multiplayer matches managed by a turn manager.
- **Online mode:** a socket server with session tokens, game rooms, friends, chat and live notifications.

## Run
Open it as a Maven project with JDK 17 and run `view.Main`. For the online features, start `server.Server` first.

## Layout
```
src/main/java/model/        buildings, people, match, map and game state
src/main/java/controller/   menu and game logic
src/main/java/view/         JavaFX screens and animations (including online menus)
src/main/java/client, server/  networking: client, server, rooms, requests, messages
src/test/java/              JUnit tests
```
