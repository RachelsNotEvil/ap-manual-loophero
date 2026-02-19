# Loop Hero
## A Manual Archipelago implementation by Rachel'sNotEvil

## Overview
This is a way to play Loop Hero in an Archipelago multiworld based on the Manual for Archipelago tools. If you don't know what any of that means, I recommend going to archipelago.gg where they explain it better than I can.

Play through Loop Hero (currently only chapter 4) as your chosen class with your maximum number of loops per run, equip slots, cards, and supply items randomized in the pool. You start with a minimum-viable 7-card deck, 1 loop, and 1 supply capacity, and must find the rest. You send checks by placing, transforming, or manifesting each kind of tile, for killing each kind of enemy, and for performing other tasks that interact with the tiles' unique mechanics. Win by defeating Omega at the end of Chapter 4.

### Setup
For information on how to set up a manual apworld, I recommend their own documentation, or you can check out my attempt to explain it [here](https://github.com/RachelsNotEvil/ap-manual-loophero/blob/main/manual_loophero_rachelsnotevil/docs/setup_en.md).

This is intended to be played with a clear save file, or at least one with access to chapter 4, with each kind of building and each card unlocked. If you're playing with level-up checks enabled, you should also have every skill unlocked by beating the game enough times.

The first thing to do is create an empty supply loadout. Since you do not start with any supply items, this is the loadout you will use to begin with. When you generate the game, it will give you items representing your character class, 1 loop, 1 supply capacity (explained below), and the 7 cards in your starting deck. You can then check these items and make your starting deck out of those first 7 cards. **If the game fails to give you enough of the right kind of cards to create a valid deck at the start, this is an error and you should notify me on the game's post in the Manual for Archipelago discord.**

**Note:** The apworld currently only supports chapter 4, and may break if you play other chapters.

## Items
### Equip Slots
A character's 4 equip slots are unavailable at the start of the game. As soon as you receive an equip slot, you may put equipment in it immediately. The equip slot given to the player by the Arsenal card is not randomized, and is unlocked simply by owning that card.

### Loops
You start the game with 1 loop, and items giving you more loops are in the pool. These items will specify in their name how many loops they give you. When the loop counter in the game exceeds your current loop total, you must end the current run. If you get every item, you will accumulate a total of 25 loops.

### Cards
You start with a minimum viable deck of 7 cards. Certain cards are omitted from being available at the start because they require other cards to be added to the deck and can cause invalid starting decks. At any time you can change up your deck, but you can only include cards that are in this 7-card starting deck or any you have found or recieved as items in the multiworld.

### Supply
Each kind of supply item appears once in the pool, and you begin with 1 "Progressive Supply Capacity". You can equip up to your progressive supply capacity of *each* unlocked supply item. For example, if you have "Antique Shelf" and "Silverware" and 3 "Progressive Supply Capacity", that means that you can equip *up to 3* Antique Shelf and *up to 3* Silverware.

### Traps
There is currently only one trap, the Hands-Off Trap. Receiving this trap means you cannot change equipment, play cards, etc. until you finish a loop by returning to the camp tile. If you're halfway through a loop, you just have to reach the camp, but if you're *already at the camp*, you need to complete the whole loop and reach camp again. Recieving this trap while not in the middle of a run applies it to the first loop of your next run, and receiving one while still resolving another hands-off trap will apply it to the *next* loop – in other words, multiple hands-off traps have to be resolved consecutively.

## Locations
### Kill
You send these checks when you kill each enemy type. You do not have to survive the battle, and if you're fast, you may claim this check before the battle is finished. Scorch Worms are an exception – you do not need to actually "kill" a Scorch Worm; causing it to run away is sufficient.

Several annoying or difficult enemies can have their locations disabled in the yaml, and several of these are disabled by default. You can defeat other difficult enemies by using the archers near the camp, but for any enemy that you cannot easily control the location of, you will be expected to have an equip slot or two before killing them.

### Level
If you enabled these locations, every skill that can be learned by leveling up is a check. This turned out to often hide important items behind a lot of tedium and rng, so I don't recommend this unless you're playing an async where everyone is picking awful settings.

### Placement
You send these checks when you place a tile using a card. You still get the check for the basic tile even if that tile immediately transforms.

### Transformation
You send these checks by transforming a tile into the tile listed in the name. This is **not** the name of the tile it transforms *from.* For example, you get the check "Transform Ransacked Village" when you transform a village into a ransacked village, not when you transform a ransacked village into count's lands.

### Manifestation
This is my name for when the game places a tile for you when you meet certain conditions, such as when "A Village?" appears when you place enough forest or thicket tiles. The starting road tiles, "Wasteland", are placed automatically by the game, so they go into this category. Think of it as a free check at the start of your first run.

### Tasks
These are various interactions with the unique mechanics of a tile that didn't fit into any other category. I'm hoping to add a lot more Tasks in the future.

### Boss
This is a subset of the "Kill" category that includes only the 4 bosses.

### Tile
This is a catch-all category that combines Placement, Transformation, and Manifestation locations.

## General Tips
Don't forget to claim your "manifest wasteland" at the start of your first run!

It can be hard to tell when certain enemies appear, particularly if you're relying on archers in the early loops or have the battle speed turned up. Some things I've found helpful are:
The Chest and Mimic look different when defeated: the Chest just looks like an open chest, while the Mimic is sagging and distorted.
Ghosts make a unique sound when they appear.

GLHF!