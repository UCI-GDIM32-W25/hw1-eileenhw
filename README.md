[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/MjLLqDcN)
# HW1
## W1L2 In-Class Activity
Game Objects
- UI (Seeds planted text and seeds remaining text)
  - Does not decrease past 0
  - Seeds planted does not increase past the original remaining seeds number
- Player
  - Action: 
    - movement with WASD
    - put down plant with space
  - Very cute :D
- Plants 
  - Appears at the position the player is at when space is pressed
  - Appears on top of player
  - Cannot place down after number of seeds remaining is 0
  - Can overlap 
  - When SPACE: increase planted count and decreases seeds count

Scripts/Classes
- Player (actions: movement and planting)
- UI update 

Potential improvements:
- Restart game
- Indication for overlapping plants?
- Player animation when moving
- End game after all seeds are planted
- Add world bounds

## Devlog
During the in-class activity, we mostly specified the behavior of the player and UI. The elements such as scripts for player (Player) and UI update(PlantCountUI), character, and UI text were pre-created. I chose a plant different from the demo to add as the prefab. I managed to get movement (WASD for movement in the player class) to work based off what I remembered from GDIM31 and started setting the UI text, in the breakdown I noticed there were 2 UI texts the plant count and the seed count which are _numSeedsleft and _numSeedsPlanted.  Based on the observations, I also added an on-input for the space so when the spaced is pressed the PlantSeed() function runs and increment changes to the count variables. When space is pressed the plant count increases and the seed count decreases. Next I implemented the plant seed system, which adds a plant at the player's location. I used unity documentation for the Instantiate() function and figured out that it allows for a Vector3 location as an argument using Instantiate(prefab,position,Quaternion.identity). One difference from what we wrote down vs the outcome is that I didn't implement any potential improvements since it wasn't required. Overall I remembered most of the conceptual stuff like conditional statements, functions, and movement the best and forgot more of the specific functions and how to use them. 

## Open-Source Assets
If you added any other outside assets, list them here!
- [Sprout Lands sprite asset pack](https://cupnooble.itch.io/sprout-lands-asset-pack) - character and item sprites

## Prof comments
I believe you managed to link your break-down to your code here, but I would be super careful next time to read the Devlog prompt and make sure it's EXTREMLEY clear that you've answered it.

For example, I am interpreting this line:

> in the breakdown I noticed there were 2 UI texts the plant count and the seed count which are _numSeedsleft and _numSeedsPlanted.

To mean that you are describing the way that you implemented the UI in Unity based on the two objects you listed in the breakdown for the UI. However, I would have liked you to elaborated on this with something like "I implemented the two UI objects mentioned in the breakdown as two different GameObjects in the Hierarchy with Text Mesh Pro Text Componenets", and then elaborated on how _numSeedsLeft and _numSeedsPlanted were used in the code to change the Text values on these Components. Although I can give you full points for this Devlog, in HW2, make sure to be more specific and thoroughly address the Devlog prompt to ensure you continue to earn full marks!

Please consider formatting your break-down activities with the hyphen '-' symbol as suggested above, and remove the prompts. This will make it a lot easier for me to read. See the [README formatting guide here](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).
