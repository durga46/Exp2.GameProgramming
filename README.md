# Ex No :02

# <p align="center">  Player movement</p>

## Aim:
To Create a player movement using pawn,collectable,player health and score.

## Software Required:
Unreal Engine.

## Procedure:
To create a player movement using a pawn, collectibles, player health, and score in Unreal Engine, you can follow these steps:

### Create the Pawn Blueprint:

In Unreal Engine, go to the Content Browser and right-click to create a new Blueprint class.
Choose "Pawn" as the parent class and name it "PlayerPawn" or any desired name.
Open the PlayerPawn Blueprint and go to the Event Graph.

### Implement Player Movement:

In the Event Graph, right-click and search for "InputAxis MoveForward" and "InputAxis MoveRight" nodes.
Connect these nodes to the corresponding inputs of the "Add Movement Input" node.
Connect the "MoveForward" node to the "Forward/Backward" input of "Add Movement Input" and "MoveRight" to the "Right/Left" input.
Connect the "Add Movement Input" node to the "Set Actor Location" node, connecting the output execution pin to the input execution pin of "Set Actor Location."

### Implement Collectibles:

Create a new Blueprint class, choose "Actor" as the parent class, and name it "Collectible" or any desired name.
Add a static mesh component to the Collectible Blueprint and assign it a mesh or shape
.
### Implement collision handling to detect when the player touches the collectible:
Right-click in the Event Graph and search for "On Component Begin Overlap" node for the static mesh component.
Connect the "On Component Begin Overlap" node to a custom event, e.g., "Collect."
Inside the "Collect" event, add logic to increment the player's score and destroy the collectible actor.


### Implement Player Health:

Inside the PlayerPawn Blueprint, create a variable named "Health" of type float.
Add logic to handle player health, such as decreasing the health when the player collides with enemies or other damaging objects.
You can use "On Component Begin Overlap" nodes or custom events to detect collisions and decrement the health variable.
Implement logic to check if the player's health reaches zero or below, and handle the game over state accordingly.

### Implement Score:

Inside the PlayerPawn Blueprint, create a variable named "Score" of type integer.
Increment the score variable whenever the player collects a collectible.
You can add a text widget to the UI and update it with the current score using the "Set Text" node and "Score" variable.


### Spawning Collectibles:

In your game level Blueprint or a separate Blueprint, implement logic to spawn collectibles at regular intervals or specific locations.
You can use the "Spawn Actor" node to create instances of the Collectible Blueprint in the world.


### Player Input:

In the PlayerPawn Blueprint, you can handle other player inputs such as jump, crouch, or any additional movements based on your game requirements.
Remember to save and compile your Blueprints after making changes. You can also add additional functionalities and customize the behavior of collectibles, player health, and scoring based on your game design.

## Output:
![WhatsApp Image 2023-06-01 at 9 36 09 AM](https://github.com/durga46/EX1.game-programming/assets/75235704/f463c951-c057-4019-9615-dc2342281bf2)


## Result:

Thus to Create a player movement using pawn,collectable,player health and score done successfully in Unreal Engine





