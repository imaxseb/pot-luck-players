# Pot Luck Players

## Introduction

This is to run sweepstake competitions where each person gets a random selection of players.

Multiple prizes can be won throughtout the whole tournament and each person should have a more equal chance of winning
compared to each person getting one or two teams. Due to the number of players the 
sweepstake can be scaled to many more people entering.

Each person will be assigned an equal number of people, any additional players will be noted as spares.

## Prize Suggestions

Prizes can be awarded for any player. Some suggestions are:

- First goalscorer
- Last goalscorer
- First yellow card
- First penalty save

## Setup & Running

1. Set variables in`setup.py`.
   1. `TOURNAMENT` The name of your sweepstake.
   2. `POSITIONS` A list of the positions, in order, used in the squad list.
2. Run `setup.py` to create a folder for the sweepstake.
3. Create a file called `people.csv` in the folder created in step 2 listing all the
people entering.
4. 
   1. Create a file called `squads.csv` with the following columns:
       - **Position** One of the options set in step 1 ii.
       - **Player** Name of the player.
       - **Team** Team of the player.
   2. A `squads.csv` for the FIFA World Cup 2022 has be made available.
5. Run `main.py` which will output the following files:
    - `pot_luck_players.csv` List of all the players and which person has been assigned to them.
   The columns will be sorted in the following order:
      - Person
      - Team
      - Position
      - Player
    - `pot_luck_players.html` As above in html format.
    - `person_position.csv` A breakdown of how many players of each position each person has.
    - `person_team.csv` A breakdown of how many players of each team each person has.