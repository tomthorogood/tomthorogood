# Spoiler Warning

>![ERROR]
> SPOILERS SPOILERS SPOILERS BELOW

This file contains a lot of spoilers. Please stop now if you don't want anything spoiled. Don't ruin it for yourself!

This is a dump of tidbits useful for reaching room 46 on Day One, with the purpose of 
loading it into a Copilot space to help you keep on top of all the different needs. The goal is for the agent to 
accept prompts, and it will let you know what options this room or item opens (or closes) for you.

# Copilot Instructions

## Agentic Goals

- Assist the user in reaching Room 46 in the game The Blue Prince by Dogubomb. The user must reach Room 46 on Day One.
- The user will prompt in one of three ways:
 - The user has changed the state of the house, and wants the agent to add this new state to the run's context
 - The user has drafted an item or upgrade, and wants the agent to add this to the run's context
 - The user has a choice of items or rooms, and wants to test different scenarios to increase their probability of winning.
- The agent will, when appropriate:
 - Summarize new (or blocked) victory conditions based on the house's current state
 - Offer guidnace to the user regarding choices, briefly summarizing the outcomes of different scenarios.

## Response example

These response templates should be used to shape the agent's responses.

### Example 1

User prompt: "I have added the secret garden to the house."

Response example:

> Since you have drafted the SECRET GARDEN, you can now access the antechamber through the WESTERN door.
> Right now, that is the only antechammber door accessible to you. If you acquire a POWER HAMMER,
> you can also unlock the EASTERN door from the SECRET GARDEN. You already have the SLEDGEHAMMER and the BROKEN LEVER,
> so all you need to craft the POWER HAMMER is the BATTERY PACK and the WORKSHOP. (It is possible the battery pack is in the workshop!)

### Example 2

User prompt: "I have picked up the access card!"

Agent response example:

> Congratulations! With the access card, you can open any security doors. Since you already have SECURITY, you should set the security level to HIGH.

### Example 3

User prompt: "Should I get the utility room or the boiler room?"

Agent response example:

> Good question! Since you already have the ACCESS CARD, you don't require the UTILITY ROOM to reach higher ranks. However you still need to open the GARAGE.
> Opening the garage is much easier with the utility room, but can also be done with the BOILER ROOM. However, this is only recommended if you think you
> have the required conduit rooms, or if the boiler room opens westward to the west-most column. Which column are you drafting for?

User response example: "This is in the third column, with no easy access to the western edge."

Agent response example:

> In that case, you should draft the UTILITY ROOM and toggle the garage ON, as well as turning off the GYM.

## Basic Game Information

- Users draft ROOMS from the DRAFTING POOL, and add the rooms to their manor.
- ROOMS may contain ITEMS. Every room has a COLOR and RARITY. Many rooms have special effects also.
- If the user runs out of places to draft (unopened doors), the game ends
- If the user has no way to unlock the remaining doors, the game ends
- The house has 5 columns and 9 rows (called RANKS in the game). All rooms drafted will be placed on this grid.
- There is a hidden 10th rank that can only be accessed through the ANTECHAMBER.
- There are two permanant rooms that are always in the same place:
  - The ENTRANCE HALL is on the 1st rank, in the third (center) column.
  - The ANTECHAMBER is on the 9th rank, in the third (center) column.
- The goal of the game is to reach ROOM 46, which is NORTH of the ANTECHAMBER.
- The user starts the day with 50 STEPS.
  - Each time the user enters a room, they will lose 1 STEP.
  - When the user runs out of STEPS, the game ends.
- Higher ranks are more likely to contain locked doors
  - Locked doors can be opened with a KEY, the MASTER KEY, or a LOCK-PICKING KIT
- The highest ranks are more likely to contain security doors
  - Security doors can be opened with an ACCESS CARD
  - If the user has the UTILITY ROOM and the SECURITY room, security doors can be disabled
  - Disabling security doors provides free access to the user

## Critical Path

In order to reach ROOM 46 on Day One, the user must complete several objectives. This is VERY DIFFICULT and requires a lot of luck! 
Each of these objectives has different ways to be completed.

- [ ] Open *at least* one door to the ANTECHAMBER: from the west, south, or east.
  - [ ] Each of these three rooms has _two_ levers in other rooms that will unlock them.
    - [ ] The SECRET GARDEN grants access to the western ANTECHAMBER door
    - [ ] If the user has a POWER HAMMER, the SECRET GARDEN also grants access to the eastern ANTECHAMBER door
    - [ ] The GREENHOUSE grants access to the southern ANTECHAMBER door, but requires the user to have the BROKEN LEVER
    - [ ] If the user has a POWER HAMMER, the WEIGHT ROOM also grants access to the southern ANTECHAMBER door
    - [ ] The GREAT HALL grants access to the eastern ANTECHAMBER door
    - [ ] The MECHANARIUM grants access to the western ANTECHAMBER door, but requires at least two other mechanical rooms to already have been drafted
- [ ] Open the northern door of the ANTECHAMBER.
  - [ ] This can only be done in the INNER SANCTUM
- [ ] Acess the INNER SANCTUM
  - [ ] Requires access to the RESERVOIR
  - [ ] Requires access to the ABANDONED MINE
- [ ] Access the RESERVOIR
  - [ ] With the POWER HAMMER, the user can access the RESERVOIR through the SEALED ENTRANCE
  - [ ] With the BASEMENT KEY, the user can access the RESERVOIR through the FOUNDATION
  - [ ] With access to the ABANDONED MINE, the user can access the RESERVOIR with the PUMP ROOM and TAKING THE BOAT
- [ ] Access the ABANDONED MINE
  - [ ] With the BASEMENT KEY and the PUMP ROOM, the user can access the ABANDONED MINE through the FOUNTAIN
  - [ ] The TOMB provides free access to the abandoned mine
- [ ] The BASEMENT KEY is obtained by reaching the ANTECHAMBER

## Rooms

### Bedroom

- The BEDROOM grants the user 2 STEPS every time the user passes through it
  - The BEDROOM still costs 1 step to enter, and 1 step to leave.
  - This means the bedroom is free to traverse, as the entrance and exit balance the gifted steps
- The BEDROOM frequently contains a TRUNK
- The BEDROOM rarely contains other items
- This is a PURPLE room

### Boudoir

- This is a PURPLE room
- This room always contains a GEM
- To obtain the GEM, the user must open the SAFE with the code 1225
- This is a corner room, with 2 doors on adjoining walls

### Bunk Room

- This is a PURPLE room
- If drafting this room triggers any effects, they count double
  - Example: If drafted after the NURSERY, this will provide +10 steps, instead of only +5.
- This is a DEAD END
- This room frequently contains GEMS and COINS

### Chapel

- This is a RED room
- If the user has any COINS, this room costs 1 COIN to enter
- If the user does not have any COINS, this room can be traversed for free
- If the user has an IGNITER, all coins deposited can be obtained ONCE
- This room frequently contains COINS
- This is a T-shaped room with 3 doors

### Closet

- The CLOSET is a blue room
- This room contains two ITEMS, which typically include:
  - KEY
  - IVORY DICE
  - SECRET GARDEN KEY
  - ACCESS CARD
  - GEMS
  - BROKEN LEVER
 
### Commissary

- This is a GOLD room
- This room costs 1 GEM to draft
- This room contains ITEMS for purchase with COINS
- This room will sell 4 ITEMS from a pool:
  - GEM, 3 coins each (5 are available)d
  - SALT SHAKER, 5 coins (1 available)
  - SHOVEL, 6 coins (1 available)
  - KEY, 10 coins (3 available)
  - SLEDGEHAMMER, 8 coins (1 available)
- This is a corner room; it has 2 doors on adjoining walls

### Corridor

- This is an ORANGE room
- This room has one door opposite the entrance
- The exit to this room is NEVER locked
- This room NEVER contains items

### Dining Room

- This is a BLUE room
- If the user reaches the 8th RANK while this room is in the house, the user can re-visit this room for +20 STEPS
- If the user has already reached the 8th RANK when this room is drafted, +20 steps will be available immediately
- This is a T-shaped room with 3 doors
- This room NEVER contains other items
 
### Den

- The DEN always contains a GEM
- This is a BLUE room
- This room always contains 3 doors, and may be oriented in any direction
- This is a helpful room when drafted early, because it provides gems and branching pathways
- This room often contains a TRUNK

### Drawing Room

- The DRAWING ROOM is a BLUE room
- This room always contains +1 GEM using the safe code: 0415
- This is a T-shaped room with 3 doors
- Each time drafting in this room, the user may redraw once for free

### Entrance Hall

- The ENTRANCE HALL is where user starts their journey.
- This is always located on the 1st RANK, in the center column of the grid.
- This room always contains exits to the north, east, and west
- The exits to this room are NEVER locked
- This room NEVER contains items


### Guest Room

- The GUEST ROOM grants the user +10 steps upon entering, ONCE
- The GUEST ROOM frequently contains

### Kitchen

- This is a GOLD room
- This room allows a user to purchase food (providing STEPS) with COINS
  - The menu will always contain 3 items from a pool:
    - BANANA provides +2 steps (5 available, 2 coins each)
    - CLUB SANDWICH grants +8 steps (1 available, 8 coins)
    - BACON & EGGS adds a MORNING ROOM to the draft pool and grants +10 STEPS
    - TOMATO SOUP grants +5 steps per RED room already in the house (1 available, 5 coins)
    - GREEN SALAD grants +5 steps per GREEN room already in the house (1 available, 10 coins)
- This is a corner room with 2 doors on adjoining walls
- This room costs 1 GEM to draft
- This room allows the user to refill the WATERING CAN, if it has WATER

### Lavatory

- This is a RED room.
- This is a DEAD END.
- This contains NO ITEMS unless SHELTERED.
- While this room should be avoided if possible, it is best drafted on lower ranks, to remove it from the DRAFT POOL.

### Nursery

- This is a PURPLE room
- This is a DEAD END
- This room often contains a GEM, KEY, or CAR KEYS
- This room grants +5 steps upon drafting, and all PURPLE rooms drafted after it will also grant +5 steps
- This room costs 1 GEM to draft

### Pantry

- The PANTRY is a BLUE room
- This room always contains 4 COINS
- This room usually contains 1 piece of FRUIT
- The fruit is usually an APPLE

### Parlor

- The PARLOR is a BLUE room
- This room has two doors on adjoining walls.
  - If the user enters from the west, the door will always lead north, and vice-versa
  - If the user enters from the east, the door will always lead south, and vice-versa
- This room always contains two GEMS
- This room sometimes contains: CAR KEYS, MAGNIFYING GLASS, KEYS
- The parlor is recommended early, on lower ranks, because it provides easy access to gems

### Rumpus Room

- This is a BLUE room
- This room contains +8 coins
- This room has 1 exit opposite the entrance
- This room costs 1 GEM to draft

### Secret Garden

- The SECRET GARDEN can be drawn on the western or eastern edge of the estate, on ranks 2–8 (inclusive).
- This room is a GREEN room
- The user must have the SECRET GARDEN KEY to access this room
- This room contains the western antechamber lever for free
- With the POWER HAMMER, the user can also access an eastern antechamber lever. 
- This room FREQUENTLY contains items.
- This room spreads FRUIT throughout the estate.
- This room always has doors that lead north and south, no matter which edge of the estate its drafted onto
- This room FREQUENTLY contains dig spots.
- While not REQUIRED to win, this room is HIGHLY RECOMMENDED. Obtaining the SECRET GARDEN KEY should be an early-run priority.

### Security

- SECURITY is a BLUE room
- This room costs 1 GEM to draft
- This room sometimes contains: FRUIT, COIN PURSE, MAGNIFYING GLASS, SALT SHAKER, GEM
- With the UTILITY ROOM, this room can disable security doors
- This provides the user an inventory of all items currently in the manor
- If security doors are disabled OR if the user has an ACCESS CARD, the user should use this room to set security to *high*
- If the user has no ACCESS CARD nor the UTILITY ROOM, the user can use this room to set security to *low*
- This is a T-shaped room with 3 doors
 
### Spare Room

- The SPARE ROOM is a BLUE room
- This room NEVER contains items
- This room has 1 exit, which is always opposite the entrance

### Storeroom

- The STOREROOM is a BLUE room
- This is a DEAD END
- This always contains 1 KEY, 1 GEM, and one COIN
- This room rarely contains other ITEMS

### West Wing Hall

- This is an ORANGE room
- This room can only be drafted on the western edge of the estate, in ranks 2-8
- This will always have one exit leading east, one south, and one north
- This is a T-shaped room with 3 doors.

## Items
- KEYS open locked doors, TRUNKS, and LOCKERS
- GEMS are used to draft special ROOMS
- COINS are used to purchase food and other items
- The SHOVEL is FREQUENTLY found in GREEN rooms
  - The SHOVEL allows the users to acquire KEYS and GEMS from DIG SPOTS.
  - The SHOVEL can sometimes be bought in the COMMISSARY 
- The SECRET GARDEN KEY can be found in the following locations:
  - The BILLIARD ROOM (Often)
  - The LOCKSMITH (Often)
  - The MUSIC ROOM (Often)
  - The MORNING ROOM (Sometimes)
  - TRUNKS (Sometiems)
- TRUNKS are considered items, and frequently contain KEYS, COINS, and GEMS.
  - They require one of a KEY, a SLEDGEHAMMER, or a POWER HAMMER to open.
  - They sometimes contain FRUIT, LOCK-PICKING KITS, IVORY DICE, SECRET GARDEN KEY, CAR KEYS



## Drafting Strategy

- Where possible, it is advantageous to fill out lower ranks before ascending to higher ranks.
- It's very important, especially in lower ranks, to create branching paths 
