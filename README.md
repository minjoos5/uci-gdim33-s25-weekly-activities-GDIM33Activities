# GDIM 33 In-Class Activities
## W1
### Activity 1


<img width="2844" height="3538" alt="canvas_gdim-33-260402_0129" src="https://github.com/user-attachments/assets/b73fc58d-e90c-4829-9514-6931425c501e" />

1. 
- My game idea is a 3D first-person perspective horror game with a crime/backroom theme. The patterns found in my moodboard are nostalgic circumstances, violent themes, and unpredictable psycho enemies. The game mechanics will involve avoiding the enemy, using retro items to fight against & escape from the backroom.
2. 
- The similarities between my teammate and me were that we both focused on the horror genre game. Compared to my game, my teammate (Milla)'s game is about a point-and-click visual novel with detailed dialogues. Her game mechanics are based on conversation, navigation, and slay-the-princess style (psychological, eerie theme). The differences between us were the focus of the player's sense of immersion. Milla focuses on psychological experiences, while I focus on physical suspense and action.
3. 
- LA Eric shared his favorite games. His favorite game genres are FPS and multiplayer cooperative games. My taste is opposite to his favorites, but he mentioned he also enjoys some horror games like GTFO.
- FPS, multiplayer corporation games, Deep Rock Galactic + GTFO


### Activity 2


![GDIM 33-1](https://github.com/user-attachments/assets/37a5d072-2589-45a3-8ae2-71df7f3093a1)

## W2

Activity was updated on GitHub.

## W3

### Activity 1

<img width="2384" height="2187" alt="IMG_0656" src="https://github.com/user-attachments/assets/d38c3ac5-a143-40d4-b0a8-9307aa6309bb" />

### Activity 2

1. I was able to call the scene variable from a different graph. Thus, I could manage events across multiple graphs, such as serializing a field or a locator. I was able to call the clickNpcEventName event in the Walrus visual script.
2. It was useful to use debug log nodes in the in class activites since I was able to check which feature is working or not. I could review the graph with the problem and fix it comprehensively.
3. It's relevant to my vertical slice since my vertical slice is a point-and-click horror adventure game. The cursor should be in the middle and fixed so that the player can know where the cursor is (to identify its location, I put the white crosshair in it)
Is the concept of a "game state" relevant to your Vertical Slice? Why or why not?
4. I think the game state will be relevant to UI, deciding when to show the appropriate UI window. Based on the game state, the UI manager will display the appropriate UI screen to depict the character's situation. (game over screen with restart button, game win screen, game start screen, and more.)

## W4
### Activity 1
What’s playable:
- The player can pick up items (the item disappears when the player clicks it)
- The player can run from the NPC and hide
- NPC follows the player and shows the game-over screen when the player collides with the NPC


Playtest goal:
- Check the game experience & movement
- Is there any error?
- What can I improve?


Playtest notes: (Ruth & Eli)
- Mouse sensitivity is too high
- The player’s speed is too high
- The playtesters had difficulty understanding the goals and interactive items	
- Recommended adding simple text like (click to interact) with the items
- I think I can add glow/color/other VFX to the interactive items
- Manipulate the timing of the monster's appearance so the player can investigate the backroom in detail.
- Besides this, everything is okay

### Activity 2
1. I think they can use these visual scripting graphs to design nodes. However, I think they must write at least some code to make the diagram work since all visual scripting graphs and scripts require programming knowledge. If the writer has a background in programming, then yes.
2. If the scripts get longer, the writer has to make a number of nodes, which is not scalable and redundant. It’s better to use another program to make longer dialogues.
3. Resetting the node system to use new nodes

## W5

### Activity 1

Navmesh for NPC chasing

1. Call NavMesh in Unity and select the game object that will serve as the ground (the area where the NPC will navigate).
2. Bake the navmesh first to check the NPC’s movement.
3. In C# or visual scripting, put a navmesh agent.setDestination(player transform) to make the NPC follow the character.
4. However, the NPC won’t be able to detect the obstacles, and it’ll try to approach the player, ignoring any obstacles in front of it.
5. Once this works, then go to Navmesh (obsolete) to make the NPC detect the walls (or other obstacles)
6. Check navigation static, generate off-mesh links. Set the navigation area not walkable.
7. Now, connect the raycast to make the NPC detect the player with its own sight system.
8. The NPC will use raycast and gizmos to check whether it’s raycast from its eye part (if it’s humanoid). If the raycast works okay, disable the gizmos in the script and write the sight system script. (the length of the ray, the distance between them, and how sight connects to the previous state machines/distance detection)
9. Then the NPC will detect the obstacles with its sight and follow the character based on the transform input at the end.


### Activity 2

- The NPC moves around the map, following the player’s transform.position.
- The NPC detects the wall and avoids it.
- The NPC changes state based on the distance between the player and itself.
- The NPC has the sight on its chest. It plays the warning sound when it sees the player.


## W6
### Activity 1
#### New updates
- The stamina bar was added
- The enemy now has the hit animation
- The enemy detects the player with the raycast, not the distance between the player and the NPC


#### [Itch link](https://minjoos5.itch.io/gdim-33-milestone-2)

#### The goals
- Check these items below:
  - Does the enemy’s raycast work okay?
  - Does the stamina work well? Is it buggy?
  - Does the hit animation show at the appropriate moment? (when the player stabbed the NPC with the knife item)


#### Playtesting Notes
- The wall is too sticky (stuck)
- It’s difficult to compare which one is a clickable item or an interactable item
- Want to see the map again (the player has to go to find a cassette player to see the map again)
- The enemy's movement and raycast system were good & stamina is too much (if I make the enemy faster, it might change)
- Maybe improve the balance between the enemy and the player’s speed (stamina system)


### Activity 2
1. Since the multiply option literally multiplies the RGB values of two vectors, it results in a darker material color. (The number will become larger if the two vectors’ values are multiplied.)
2. Less translucent means the alpha value determines transparency; it is also multiplied (unless it’s a negative value, the value will decrease as it’s multiplied)
3. From the vectors of the Shiba
4. Yes! It’s because I’ve always wondered about the differences between the layer effects in drawing tools (overlay, multiply, screen, etc.).
