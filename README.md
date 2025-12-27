# 🎮 SeedOfLife_Pico8
A top-down farming game made with the fantasy console PICO-8, where you play as a robot trying to grow and harvest crops in a ruined world.

## 🛠️ Technology
- `PICO-8`
- `Lua`

## 🚀Features
- **Top-down movement -** freely wander the ruins and choose the best spots to plant crops.
- **Timer/Battery Management -** every action and movement drains a limited battery reserve, creating strategic tension so the player must balance planting, harvesting and travel before the battery or time runs out.
- **Planting/Watering/Harvesting -** choose tiles to plant seeds; once planted, the player must water them daily until they’re ready to harvest. Timely care affects growth.
- **Buy, Plant, Sell -** the loop of the game hinges on managing resources: buy seeds, cultivate them, harvest the produce, then sell to earn coins and progress to the next day, all so that you can grow your farm.

## 🧠 Process
I started by making the tiles and sprites of the game, which includes the full growth cycle of the crops. Once the full tile set of the crops growing was created, I then moved to the creation of the character, which is a hovering robot. I then created placeholder tiles of buy, sell and charge areas that the player will interact with. 

For the hud, I started by making each icon and placed it at the very bottom of the map. To build the yellow target system, I created a yellow square and marked it as a sprite as well. Using the player’s position as reference, the yellow target is dynamically drawn at the bottom tip of the robot giving a clear visual cue for actions and targeting. 

The action button would cover many tasks, such as harvesting, watering, planting of crops, advancement to the next day, buying and selling, so each tile would have to react differently when the X button is pressed. 

The challenge game for the game would be the limited battery/time and day progression. When the robot returns to its station to recharge, the day progresses. I used a quick `rectfill` transition to simulate the day change, and tiles that met farming conditions (e.g. watered) are updated to the next growth stage.

Since there is a charging station and day system, a health charge and day timer would be the game-over decision factor. A simple black screen with a "You Lose" message is displayed when either the bot’s charge or timer drops to 0. 

## 📦 Running the project

1. Clone the repo and load the project in PICO-8 (You need to have the PICO-8 fantasy console).
2. Control the robot using the **arrow keys** to move around the ruins, use the “X” key to interact with the world!

## **🎯 Credits**

Inspired by SpaceCat’s farming game [https://www.youtube.com/playlist?list=PLavIQQGm3RCnNsa8XBNFpDY7QnawWlBPE]). Big thanks to him for the tutorial!

## 🖼️ Preview
https://github.com/user-attachments/assets/54fcb47b-5470-457a-b317-19ce9c26b156
