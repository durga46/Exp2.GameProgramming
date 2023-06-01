# Ex No 🕥3

# <p align="center"> Third person character mesh and add animations</p>

## Aim:
To Change the third person character mesh and add animations by using Unreal Engine.

## Software Required:
Unreal Engine.

## Procedure:
To change the third person character mesh and add animations in Unreal Engine, you can follow these steps:

### Replace the Character Mesh:

In Unreal Engine, go to the Content Browser and find the new character mesh you want to use.
Right-click on the new character mesh and choose "Asset Actions" > "Create Blueprint using this" to create a Blueprint based on the new mesh.
Open the new Blueprint and go to the Event Graph.

### Set up Animation Blueprint:

In the Event Graph of the new Blueprint, right-click and search for "Update Animation" and "Get Mesh" nodes.
Connect the "Get Mesh" node to the "Target" input of "Update Animation" node.
Right-click and search for "Set Anim Instance Class" node and connect it to the "Update Animation" node.
In the "Set Anim Instance Class" node, choose or create an Animation Blueprint for your new character mesh.

### Create Animation Blueprint:

In the Content Browser, right-click and choose "Animation" > "Animation Blueprint" to create a new Animation Blueprint.
Open the Animation Blueprint and go to the Event Graph.
Right-click and search for "Event Blueprint Update Animation" node. This node will execute on every frame to update the animations.
Connect the output execution pin of "Event Blueprint Update Animation" to the input execution pin of "Update Animation" in the Character Blueprint.

### Add Animations:

In the Animation Blueprint, you can create or import animations for various character actions, such as idle, walk, run, jump, etc.
Use animation nodes like "Play Montage" or "Play Animation" to trigger specific animations based on the desired character behavior.
Connect the output execution pins of these animation nodes to the appropriate input execution pins in the Animation Blueprint.

### Configure Animation Blueprint:

In the Animation Blueprint, you can modify the behavior and blending of animations using various nodes and transitions.
Use animation state machines to define different animation states and transitions between them.
Adjust blending, layering, and animation curves to achieve the desired character animation behavior.

### Assign the New Character Blueprint:

In your game level or wherever you want to use the character, drag and drop the new character Blueprint from the Content Browser into the scene.
Remove or disable the default third person character Blueprint if it's still present in the scene.

### Adjust Character Blueprint Variables and Logic:

If your new character mesh has different bone structure or names compared to the default third person character, you may need to update references in the Character Blueprint.
Check the logic in the Character Blueprint for any references to specific animations or sockets and update them accordingly.
Remember to save and compile your Blueprints after making changes. You can also further customize the character's behavior, add additional animations, or implement complex animation systems based on your specific game requirements.

## Output:
![WhatsApp Image 2023-06-01 at 9 36 09 AM](https://github.com/durga46/EX1.game-programming/assets/75235704/f463c951-c057-4019-9615-dc2342281bf2)


## Result:

Thus to Change the third person character mesh and add animations is done successfully in Unreal Engine.





