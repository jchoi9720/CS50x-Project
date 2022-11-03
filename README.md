# Lazerbeam
#### Video Demo:  <https://youtu.be/IcXodBwW6Ew>
#### Description: Bomberman type game with two players who can battle it out until one player remains!
There are two players and their input keys are different so this can be a fun multiplayer game. Originally in Bomberman games, there is an option to kick the bombs around, but in my version I decided to have the bombs static and not be moved around as I enjoy the strategy behind not being able to move bombs.
Another feature I decided was to keep player collisions on and allow the players to essentially block one another and even push each other rather than passing through one another. This was enabled so that there is more of a "battle" feel to the game where each player can try to block one another and potentially push each other towards explosions. The player collision models are circlular to keep things interesting and make this pushing aspect more challenging and dynamic.

## Scripts/Code:
Here is a list of the scripts written to create the game:
- 'AnimatedSpriteRenderer.cs' animates the sprites to loop through the different instances/images to create the movement visual effects.
- 'BombController.cs' is where everything bomb related is controlled. Here there are variables for the bomb such as fuse time, bomb amount, bomb qty, explosions, placing bombs, and destruction of tiles.
- 'DestroyedTile.cs has the destruction time for tiles being destroyed as well as the item spawnchance upon destroying each tile.
- 'Explosion.cs' works with the Animated Sprite Renderer to animate the bomb sprites. Here the explosion also has a SetDirection function to have the bomb explode out towards different directions and then is cleared/destroyed.
- 'GameManager.cs' has a list of players and checks to see how many players are alive. If the amount of players alive reaches 1 or less, the game ends and the round is restarted.
- 'ItemPickup.cs' stores the different items and adds the functions associated with each item which gets added to the player BombController script. This also detects players colliding with the items.
- 'MovementController.cs' sets the player speeds and movement functions. The DeathSequence is also called in this script when a player collides with an explosion.
- 'StartGame.cs' changes the title scene to the gameplay scene when any input is detected.

##### This game was created using Unity and VS Code for the C# scripts. This was my first game created and it was a great learning experience and introduction into C# and the Unity Engine. There are still aspects that need to be developed, but so far I am very happy with this outcome condisering it is my first game project!
