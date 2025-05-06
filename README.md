# VR_Teorija_iger
Kolokvij naloga iz teorije iger - Prisoner's Dilemma Tournament

This repository contains a simulation of a **Prisoner's Dilemma Tournament**, where various memory-based strategies—implemented as Python classes—compete against each other in repeated games.

### 📘 Overview

The project simulates a round-robin tournament between strategies, where each pair of strategies plays a 100-round iterated Prisoner's Dilemma game. The final results show how well each strategy performed across all matches.

The simulation is implemented using object-oriented Python with a clean structure for defining and extending strategies.

### 🧠 Strategies Implemented

Each strategy inherits from a base class `Strategy` and implements the `move()` method based on its internal logic:

| Strategy                | Description                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| `RandomStrategy`        | Chooses randomly between cooperate (`C`) and defect (`D`) in each round.    |
| `Pavlov`                | Repeats the previous move if the outcome was mutual (both cooperated or defected), otherwise switches. |
| `SuspiciousTitForTat`   | Starts by defecting, then mimics the opponent's last move.                  |
| `ReverseTitForTat`      | Does the opposite of the opponent’s last move.                              |

You can easily define new strategies by subclassing `Strategy` and implementing the `move()` function.
