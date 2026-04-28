## Slide 1

U4 Infiltration Glyph

Design Documentation

Quest Objective

Place soils in correct locations to visually represent the  infiltration  rate of different types

Core Concept 

Understand that the particle size of different soil types affects the rate through which water infiltrates through it.

Performance Determining Factors

Correct- all soils in correct location

Incorrect- any soils in an incorrect location

## Slide 2

Sequencing and Mechanics     (Basically the same functionality as U2/U3 Glyphs)

Player enters room 

Soil containers are always in the same location  (can be on scattered on floor, leaning up against wall, hanging on wall as shown below- whatever works best)

Pick up/Place

Player use E to pick up a soil, only one a time

Player uses E to deposit soil in glyph slot 

Player can remove pieces from slot with E

After all slots filled validation occurs (see here for answers)

Camera provides a view of all panels

Validation for correct/incorrect happens simultaneously 

Green glow around correct panel

No color change or glow if panel is incorrect

Incorrect panels ejected from slots 

Feedback given by DANI ( found here ) 

Outcome

If all Correct

Collectible piece revealed in center of room

Player grabs center piece, piece stored in DANI menu, door opens

If any Incorrect

Player returns to step 2

## Slide 3

Feedback

| GLYPH FEEDBACK: INFILTRATION |  |  |  |  |  |  |  |  |
|----|----|----|----|----|----|----|----|----|
| NO PLAYER INTERACTION |  |  |  |  |  |  |  |  |
| {If player doesn’t interact with objects around the room in 30 seconds…} DANI  \[gameplay\] I believe the stone pieces on the floor may fit into the wall panels. |  | {If player doesn’t interact with objects around the room in 60 seconds…} DANI  \[gameplay\] Perhaps you could attempt to place one of those pieces on the floor into a wall panel. |  |  | {If player doesn’t interact with objects around the room in 90 seconds…} DANI  \[gameplay\] Hey TK, place one of the pieces on the floor into a wall panel. We will observe what follows. |  |  |  |
| Once all four tiles are placed, they are checked simultaneously: |  |  |  |  |  |  |  |  |
| {If a piece is in the correct panel…}  {Animation: panel lights up} {Audio: positive sound plays} |  |  | {If a piece is in the incorrect panel…}  {Audio: negative sound plays} {Animation (Dev): Tile falls to the floor} |  |  |  |  |  |

## Slide 4

| FIRST ATTEMPT |  |  |  |  |  |  |  |  |
|----|----|----|----|----|----|----|----|----|
| {If player got 1-2 pieces incorrect on the first try…} DANI  \[gameplay\] This appears to be close to the solution, TK. Please continue trying. |  |  | {If player got 3-4 pieces incorrect on the first try…} DANI  \[gameplay\] I believe the pieces are intended to be ordered in a specific way. Keep trying. |  |  |  |  |  |
| SECOND ATTEMPT |  |  |  |  |  |  |  |  |
| {If player got 1-4 pieces incorrect on the second try…} DANI  \[curricular\] The images appear to represent the size of the particles of different types of soil. |  |  |  |  |  |  |  |  |
| THIRD ATTEMPT |  |  |  |  |  |  |  |  |
| {If player got 1-2 pieces incorrect on the third try…} DANI  \[gameplay\] I believe that was close to the correct order, TK. Keep trying.  |  |  | {If player got 3-4 pieces incorrect on the third try…} DANI  \[curricular\] This appears to be a graph that shows the rate at which water passes through soils of different types. |  |  |  |  |  |

## Slide 5

| FOURTH ATTEMPT |  |  |  |  |  |  |  |  |
|----|----|----|----|----|----|----|----|----|
| {If player got 1-2 pieces incorrect on the fourth try…} DANI  \[gameplay\] That is very close, TK. I believe you can solve it.  |  |  | {If player got 3-4 pieces incorrect on the fourth try…} DANI  \[gameplay\] Would you like me to assist, TK? |  |  |  |  |  |
| FIFTH ATTEMPT |  |  |  |  |  |  |  |  |
| {If player got 1-4 pieces incorrect on the fifth try…} DANI  \[gameplay\] I believe I have calculated the correct order for the puzzle. Allow me to assist, TK. Activating holid projector.  {Animation: pieces fly to correct locations} |  |  |  |  |  |  |  |  |

| Sure. I’m stuck.      DANI  \[gameplay\] I believe I have calculated the correct order for the puzzle. Activating holid projector.  {Pop-up:} U4 Toppo Lessons {Animation: pieces fly to correct locations} | No, I’m okay.  |
|----|----|

## Components

( Soil container + particle view of each of the 4 types of soil- could just be a stone with an image or actual containers of soil- whatever works)

Some sort of artistic representation of flow rate 

Assets are located in project under… 

Art Assets

- Glyph pieces
- Glyph wall 
- UI pop-up for using “E/Action” to pick up, 

place and drop pieces

- Collectible piece in center of room

(these should be organized from small particles to large particles)
