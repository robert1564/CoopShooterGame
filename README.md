# CoopShooterGame
Coop Shooter Game that use Deep Learning for AI Intelligence created with Unreal Engine 4.

My app exemplifies a multiplayer computer game in which I have integrated deep learning algorithms for AI control. I started by implementing the basic player movements at the code level, setting the character animations and third person camera. After setting the character I started by setting and coding a weapon and I implemented the core functionality for a target point that will be recorded at time of a hit, i.e. make a single line against the environment to find out which actor in the world was hit. Of course, here I implemented the damage that each bot will take and set an effect that the game will run at time of a received blow or a weapon effect.

  ![image](https://user-images.githubusercontent.com/52401139/134408350-841b7237-d161-4ed7-87c1-46bf1d60a637.png)

I also implemented the shake effect of the camera when player fires a weapon to give a realistic effect on the game and I made the first settings to implement the multiplayer mode to generate certain effects for both client and server parts, such as be displaying the effect when a bullet hits a player. Then I started by receiving an answer when applying damage to the pawn, for which I set a custom component that is represented by an object that is common to each actor. This is a very good part because they use components that can be used for the player and enemies. I also dealt with the death of a player and adding feedback to the current health level using a UMG.

  ![image](https://user-images.githubusercontent.com/52401139/134408506-42d1decb-23c5-40a7-baf0-b1967f839a3c.png)

  ![image](https://user-images.githubusercontent.com/52401139/134408653-89d18946-548d-463d-8f11-582f9e355038.png)


I create the artificial intelligence in the game by implementing a simpler enemy that is represented by a ball that follows you and can eventually kill you with an explosion. Then I implemented the sounds for game, e.g the sounds of footsteps, shooting with the gun. Then I created a tracker bot, for this type of enemy I used the basics to locate the player and focus on navigation and a simple behavior based on C++ code. Then I created the power system that the player has, in this way he can collect certain powers such as the super speed, in the end I made sure that this system works in multiplayer mode. I created two maps that the players can play and then I set a two game modes, one survival and a horde mode, for both modes I setted spawn points from which enemies and I made sure that a bot will not appeared near the player to give a type of response to each player.

  ![image](https://user-images.githubusercontent.com/52401139/134409005-5e52153e-94a6-4d48-bb02-691d6bdf2f4e.png)


In the end, I created humanoid enemies and zombies on which I integrated the deep learning algorithm so each enemy would learn moves from players to the parks and start to become more and more difficult to destroy after each appearance. I did this through a special plug-in (Mind Maker) that I modified, each information will be saved in a behavioral tree, an EQS (Environment Query System) in which I structured each saved information.

  ![image](https://user-images.githubusercontent.com/52401139/134409798-c06fe88e-3413-4b0a-be32-460e6d5bd87d.png)


In the development of the game I used a plug-in called "MindMaker" developed by the company NeuroStudio. This is an Unreal Engine tabplug-in used to create AI players that can explore the game. This exploration occurs in the background while the actor will stand still and accumulate information. The plug-in is based on choosing a "prize" for a certain behavior that actor wanted to get. This type of artificial intelligence is called "Deep Reinforcement Learning" and combines the neural network with a temporal learning module. The temporal learning mode used here is "Deep Q Learning". This is a powerful framework that has created a revolution in the field of robotics and AI-controlled mechanisms.

  ![Diagrama DQL](https://user-images.githubusercontent.com/52401139/134409426-1b871297-94d4-45ea-838a-551f0eb9dff1.png)
  
Full documentation here (Romanian language):

