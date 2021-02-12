# Knight's Duty
Knight's duty is a turn-based competitive free-for-all game for 2 to 6 players.

## Objective
The Goal of the game is to be the last man standing. 

You do that by attacking and hitting other players, while avoiding getting attacked and hit yourself.

## Components
+ Game Manual, 
+ Game Board,
+ 6 clans, composed each of:
	- Equipment miniatures (1 Sword, 1 Spear, 1 Bow)
	- Knight miniature
	- Battle cards (4 Full Heart, 4 Broken Heart, 4 Shields)
	- Action tokens (2 Sword, 2 Spear, 2 Bow, 2 Shield, 2 Parry, 3 Movement, 1 Inspiration)

## Setup
Each player chooses a Clan and takes its tokens, equipment and cards.

Each corner belongs to the clan that matches its colors.

Following the layout above, every player places their Knight and Inspiration token on the board, a stack of Full Heart and Shield cards next to the board, visible to other players.

## The turns
Every turn, all the players pick actions for the turn by putting their action tokens face down on the tracker on their corner, face down.
The number of actions you can do is determined by whether you have a Full or a Broken heart.

TODO: make visual for the action spots
TODO: Tracker is a thing now

Every player starts with a Full Heart, being able to play 3 actions per turn. After getting hit once, they play with a Broken Heart, being able to play only 2 actions per turn.

After every player has put their actions face down on the tracker, reveal and resolve one action at a time, following the order on the tracker.

If any player has a Broken heart, they can't act on the last action. They can be targeted and defend themselves accordingly, just can't make any action on the list below.

## Actions and resolve phase
Actions are resolved simultaneously for every player, following a priority order. 
The possible actions are the following, in the order they are resolved.
- Movement
- Swap equipment
- Defending
- Parrying
- Attacking
- Inspiration

TODO: make little tokens for the rules
#### Movement ([token][])
Movement allows that player's Knight to move on the battle field.

To make a movement action, simply place a movement([token][]) token on the tracker. Every player that has used the movement action than moves their Knight at the same time, 1 space in any direction.

You can't move into the same space as another player Knight, nor outside of the play area. Players can choose not to move their Knight it they wish.
If more than one player wants to move to the same space at the same time, they can make a gentleman's agreement over who gets to move to that space, otherwise neither moves this action.

#### Swapping equipment ([token][])
Every player has 3 possible weapons, the sword([token][]), the spear([token][]), and the bow([token][]).

To take a swap equipment action, place a weapon token that is different than the one you currently are equipped with on the tracker (you start without one).
That player than puts the new weapon miniature next to their corner, removing the old one. This is now the weapon they are equipped with.

Every weapon has a different range and chance to hit, described in details on the next section.

#### Defending([token][])
Defending increases your chances of not getting hit on a combat.

To make a defend action, place the shield([token][]) token on the tracker.
If you are a target of any attack action within this phase of the tracker, you count as *Defending* while resolving combat.

TODO: Check balance of how long defending/parrying lasts

#### Parrying([token][])
Parrying allows you to counter you opponent while in combat.

To make a parry action, place the parry([token][]) token on the tracker.
If you are a target of any attack action within this phase of the tracker, you count as *Parrying* while resolving combat.

#### Attacking ([token][])
Attacking is how you try to hit your opponents hearts.

To make an attack action, place a weapon([token][]) token equal to the one you are currently equipped with.(the one next to your corner)
Then, players that are attacking can declare their target within attack range. Each weapon has it's own range, being:
- Bow: 1 to 4 spaces
- Spear: 1 to 3 spaces
- Sword: 1 to 2 spaces
([range example][])

If there's no opponent within range, your attack is forfeit. Player's can also choose to target no one, if they wish.
Attacks can be resolved in any order. If more than one player is targeting the same opponent, they can make a gentleman's agreement over who gets to attack first, while the other players can wait for that attack to resolve to choose a new target or the same one.

A player that was defeated in combat **can** be both attacker and target until the end of the tracker phase.

To resolve combat, see the ***Resolving combat*** section.

#### Inspiration ([token][])
Inspiration allows you to tip the odds in your favor.
It can only be used if the *Inspiration token* is face-up([token][]).

Inspiration can be used while resolving a combat, both by the attacker and the target, as described in the ***Resolving combat*** section.
After it's use, turn the *Inspiration token* face-down([token][]).

Inspiration can be recovered by standing on the middle of the arena. ([token][])
If any knight lands on the space or starts it's turn on it, immediately turn the *Inspiration token* face up if it isn't already.


### Resolving combat
If an attacking player is targeting an opponent within range, a combat occurs.

To resolve it, the **targeted player** shuffles shields and hearts into a pile.
The targeted player uses Full Heart cards if they were not hit before, and Broken Heart if they were.
The amount of hearts and shields depends on the attacker's weapon, if the target is defending, and the use of inspirations.

##### The weapon:
- Bow: add 1 Heart and 3 Shields to the pile;
- Spear: add 2 Hearts and 2 Shields to the pile;
- Sword: add 3 Hearts and 1 Shield to the pile;

#### If the target is defending:
Remove 1 Heart and add 1 Shield on the pile;

#### Inspiration:
At this point, both player can choose to use inspiration, if possible.
- Attacker uses inspiration: add 1 Heart to the pile;
- Defender uses inspiration: remove 1 Heart to the pile;

#### Hit or Miss
After setting up the pile, check the cards on it.
If the pile has no Heart card, the attacker misses automatically.

Otherwise, the targeted player shuffles the pile and presents it to the attacking player face down.
The attacking player then picks a card from the pile.
If it is a Shield, the attack misses.
If it is a Heart, the attack hits.

### On a Miss
On a miss, the attack does no harm to the targeted player.
If the targeted player was *Parrying*, the attacking player fumbles and unequips their weapon.

### On a Hit
On a hit, the attack does damage to the targeted player.
If the target was playing with a Full Heart, they are now playing with a Broken Heart.
From now on, that player can make only 2 actions per turn.

If the target was playing with a Broken Heart, that player is defeated in battle.
After all combats on this tracker phase are resolved, that player removes their knight from the board and is out of the game.

## The High Ground
The center of the board holds the High Ground space, marked with a **([token][])**.
If any knight lands on that space or starts it's turn on it, it regains inspiration if spent.

## Winning
The last Knight standing is declared victorious. 
If two or more players fall in battle in the same round and no one is left standing, the match is a draw.