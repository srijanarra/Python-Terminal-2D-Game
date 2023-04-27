# Assignment 3.1

- Everything mentioned in the assignment has been implemented.
- **Bonus** :
    - King’s Leviathan Axe has also been implemented.
    - Dragon Character has been added, it can fly over walls.
    - Queen's Eagle Arrow has been added.
    - Movement avoiding walls has also been implemented.

- To run the game : `python3 game.py`
- To view replays : `python3 replay.py`  and select the replay you want to watch according to mentioned date and time.
- For Victory : All buildings apart from walls get destroyed from the map in all three levels.
- For Defeat : If all troops and King die before destroying all buildings apart from walls.

## Controls :

### Hero :

- w : move up
- a : move left
- d : move right
- s : move down
- 1 : Special Attack
- space : Normal Attack

### Barbarian :

- z : spawn at point 1
- x : spawn at point 2
- c : spawn at point 3

### Dragon :

- v : spawn at point 1
- b : spawn at point 2
- n : spawn at point 3

### Archer :

- i : spawn at point 1
- o : spawn at point 2
- p : spawn at point 3

### Stealth Archer :

- e : spawn at point 1
- f : spawn at point 2
- g : spawn at point 3

### Balloon :

- j : spawn at point 1
- k : spawn at point 2
- l : spawn at point 3

### Healer :

- y : spawn at point 1
- m : spawn at point 2
- 2 : spawn at point 3

q : Quit Game

## Assumptions :

- Rage and Heal Spell can be applied multiple times.
- The limit for troops in each level is as follows :
    - Barbarians : 10
    - Archers : 7
    - Stealth Archers: 7
    - Balloon : 5
    - Healers : 3
    - Dragon : 3
- You have to choose the type of troop movement at start of the game.
- You have to choose the hero after each level.


## Extensions

- Stealth Archer:
    - Does not deal direct damage (when it is targeted) for the first ten seconds after its spawned but can take indirect damage (when in vicinity of another troop which is being targeted by defensive buildings (wizard tower))
    - Behaves like an archer after first 10 seconds after its spawned

- Healer:
    - Can heal any friendly troops within its heal distance (7 tiles)
    - Follows the nearest troop around (heals the nearest troop when multiple troops are present)
    - Cannot heal more than the maximum health of the troops
    - Doesn't move when there are no troops present in the game

Assumption about distance calculation - Euclidean Distance