[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/MjLLqDcN)
# HW1
## W1L2 In-Class Activity

Put your notes from the W1L2 (Thurs, Jan 9) in-class activity here.
Game Objects
UI (Seeds planted text and seeds remaining text)
Does not decrease past 0
Seeds planted does not increase past the original remaining seeds number
Player
Action: 
movement with WASD
put down plant with space
Very cute :D
Plants 
Appears at the position the player is at when space is pressed
Appears on top of player
Cannot place down after number of seeds remaining is 0
Can overlap 
When SPACE: increase planted count and decreases seeds count

Scripts/Classes
Player (actions: movement and planting)
UI update 

Potential improvements:
Restart game
Indication for overlapping plants?
Player animation when moving
End game after all seeds are planted
Add world bounds



## Devlog
Prompt: Include the HW1 break-down exercise you wrote during the Week 1 - Lecture 2 (Jan 9) in-class activity (above). If you did not attend and perform this activity, review the lecture slides and write your own plan for how you believe HW1 should be built. If your initially proposed plan turned out significantly different than the activity answers given by Prof Reid, you may want to note what was different. Then, write about how the plan you wrote in the break-down connects to the code you wrote. Cite specific class names and method names in the code and GameObjects in your Unity Scene.


Write your Devlog here!
During the in-class activity, we mostly specified the behavior of the player and UI. The elements such as scripts for player (Player) and UI update(PlantCountUI), character, and UI text were pre-created. I chose a plant different from the demo to add as the prefab. I managed to get movement (WASD for movement in the player class) to work based off what I remembered from GDIM31 and started setting the UI text, in the breakdown I noticed there were 2 UI texts the plant count and the seed count which are _numSeedsleft and _numSeedsPlanted.  Based on the observations, I also added an on-input for the space so when the spaced is pressed the PlantSeed() function runs and increment changes to the count variables. When space is pressed the plant count increases and the seed count decreases. Next I implemented the plant seed system, which adds a plant at the player's location. I used unity documentation for the Instantiate() function and figured out that it allows for a Vector3 location as an argument using Instantiate(prefab,position,Quaternion.identity). One difference from what we wrote down vs the outcome is that I didn't implement any potential improvements since it wasn't required. Overall I remembered most of the conceptual stuff like conditional statements, functions, and movement the best and forgot more of the specific functions and how to use them. 

## Open-Source Assets
If you added any other outside assets, list them here!
- [Sprout Lands sprite asset pack](https://cupnooble.itch.io/sprout-lands-asset-pack) - character and item sprites
