# Spirebound

Spirebound is a lightweight, browser-based card battler inspired by Slay the Spire. It captures the feel of a turn-based deck-building encounter: build a hand, spend energy, manage block, and survive increasingly punishing enemy turns.

## Overview

You play as a lone adventurer in a hostile spire, facing enemy sentinels in a compact combat loop. Each turn you:

- draw cards from your deck
- play attacks and defensive cards
- manage energy and block
- try to outlast the enemy before your health runs out

The game is intentionally simple, fast, and playable directly in the browser without any setup beyond opening the HTML file.

## Features

- Turn-based combat inspired by deck-building roguelites
- Card-based actions such as attacks, defense, and offensive bursts
- Energy system that limits how many cards you can play per turn
- Draw and discard pile mechanics
- Block and damage resolution
- Vulnerable and enemy intent logic
- Instant replay loop with a restart button after each fight
- Fully self-contained single-file HTML game

## How to Play

1. Open `spirebound.html` in your browser.
2. At the start of your turn, cards are drawn automatically.
3. Click cards in your hand to play them.
4. Spend energy wisely to attack, block, or defend.
5. End your turn to let the enemy act.
6. Survive the enemy's attack and keep your health above zero.
7. If you lose, restart and try a different tactical approach.

## Controls

- Click a card in your hand to play it
- Click `End Turn` when you are ready to pass the turn to the enemy
- Click `Restart` after a win or loss to begin again

## Card Types

The game includes classic card-style actions similar to other roguelike deckbuilders:

- Strike: deal damage to the enemy
- Defend: gain block to reduce incoming damage
- Bash: stronger offensive option for bigger damage
- Other attack and defense cards may appear depending on the game state

## Core Game Systems

### Energy
Each turn, the player receives a fixed amount of energy to spend. Cards have costs, so you must decide which actions are worth using now and which should be saved for later.

### Block
Block reduces incoming damage before health is lost. It functions like armor, helping you survive stronger enemy turns.

### Draw and Discard
Cards are drawn from the deck into your hand, and discarded after use. When the draw pile is empty, the discard pile is reshuffled back in.

### Enemy Behavior
Enemies act based on their intent. Some attacks are straightforward, while others may favor defense or more aggressive damage patterns.

## Running the Game

Because the project is a single HTML file, the simplest way to run it is:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/spirebound.html
```

Alternatively, you can open `spirebound.html` directly in a browser.

## Project Structure

```text
spirebound/
├── README.md
├── spirebound.html
└── (future assets, scripts, or game files can be added here)
```

## Notes

This project is intentionally compact and beginner-friendly. It is a great starting point for expanding into a fuller roguelike experience with:

- more card types
- enemy variety
- relics and buffs
- map progression
- sound effects and animations
- higher-level progression systems

## License

This project does not currently include a license file. If you intend to share or distribute it publicly, consider adding a license such as MIT.

## Contributing

Contributions are welcome if you want to expand the mechanics, improve the UI, or add new content.

---

Built as a simple, browser-playable card combat prototype inspired by the rhythm and tension of Slay the Spire.
