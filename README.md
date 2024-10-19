# Aplicacion
This repository contains the python programme for the Programming applied to AI subject


# Mus Card Game Simulator
This Python project simulates the setup and gameplay for the Spanish card game "Mus," with options for different game modes using customized decks. The classes provided handle the deck's creation, card distribution, and scoring for a Mus match.

## Features
* **Customizable Decks**: Create a traditional 40-card Spanish deck or modify it for specific Mus variants (Mus with 8 kings or 4 kings).
* **Deck Shuffling**: Shuffle the deck randomly to ensure a fair game.
* **Card Distribution**: Automatically deal cards between four players.
* **Scoring System**: Keep track of points for two teams during the match.
* **Flexible Game Modes**: Play either Mus with 4 kings or Mus with 8 kings, with distinct deck setups.
## Classes
1. 'baraja()'
Represents the deck used in the game. By default, it creates a 40-card Spanish deck with 4 suits (palos).

**Parameters**:
'n_cartas': Number of cards in the deck (default is 40).
'n_palos': Number of suits in the deck (default is 4).
**Key Methods**:
'shuffle()': Shuffles the deck.
'take_card()': Draws a card from the deck.
'restart()': Resets the deck for a new game.
'introduce()': Adds a new card to the deck.
2. 'mus8()'
A subclass of baraja, this prepares the deck for playing Mus with 8 kings by modifying certain card values and shuffling the deck.

**Parameters**:
'punto_a': Points for team A.
'punto_b': Points for team B.
3. 'mus4()'
Another subclass of baraja, this prepares the deck for playing Mus with 4 kings. It shuffles the deck and keeps track of team scores.

4. 'partida()'
Handles the game mechanics, including dealing cards to four players and tracking the game score.

**Parameters**:
'modo': The game mode (mus4 or mus8) that sets the deck configuration for the match.
**Key Methods**:
'reparto()': Distributes cards to the players.
'win_a()': Adds points to team A's score.
'win_b()': Adds points to team B's score.
'puntuacion()': Prints the current score for both teams.
'restart_score()': Resets the score for a new game.
