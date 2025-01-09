[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/MjLLqDcN)
# HW1
## W1L2 In-Class Activity

Put your notes from the W1L2 (Thurs, Jan 9) in-class activity here.

## Devlog
Prompt: Include the HW1 break-down exercise you wrote during the Week 1 - Lecture 2 (Jan 9) in-class activity (above). If you did not attend and perform this activity, review the lecture slides and write your own plan for how you believe HW1 should be built. If your initially proposed plan turned out significantly different than the activity answers given by Prof Reid, you may want to note what was different. Then, write about how the plan you wrote in the break-down connects to the code you wrote. Cite specific class names and method names in the code and GameObjects in your Unity Scene.


Write your Devlog here!
Started coding with what I remembered from GDIM 31 to see what I retained. From this, I managed to get movement to work and started setting the UI text. I remembered needing to use the transform and translate but didn't fully recall the entire code so I had to test around a bit until I figured out the Vector3 and Time.deltaTime stuff. I also added an on input for the space so when the spaced is pressed the PlantSeed() function runs and increment changes to the count variables. I then had to reference the blob battle project from last quarter to add the UI text, since I got an error that the text has to be a string and can't just be the int value I added""+ to the text. The part that I forgot getting the prefab to spawn, I knew I had to use Instantiate to create the copy of the prefab but had slight trouble figuring out how it could spawn on the position it needed to be. I used unity documentation for the Instantiate() function and figured out that it allows for a Vector3 location as an argument using Instantiate(prefab,position,Quaternion.identity). I learned that Quaternion.identity keeps the default rotation. So to get the position, I tried getting the playerPosition which was much simpler than I expected because I tried creating a Vector3 by setting each axis instead of just using .position. Overall I remembered most of the conceptual stuff like conditional statements, functions, and movement the best and forgot more of the specific functions and how to use them. 

## Open-Source Assets
If you added any other outside assets, list them here!
- [Sprout Lands sprite asset pack](https://cupnooble.itch.io/sprout-lands-asset-pack) - character and item sprites
