# Text-Based-RPG
A short text based RPG

## Overview

This is a text-based role-playing game (RPG) built in Java that allows players to explore a series of interconnected rooms in a house.
Each room contains items that can be picked up or dropped, and rooms may have unique mechanics (such as healing).
Players can navigate using typed commands and manage an inventory system.

🧩 Features

    🧍 Player creation and inventory system

    🧭 Room navigation with cardinal directions (north, south, east, west)

    🪑 Dynamic room objects and interactions

    🛏️ Special rooms (e.g., Sleep Room that heals the player)

    🛠️ Command-based interaction system (like look, inventory, pick up)

    📦 Utility class for modular string-based item management


🎮 Gameplay

You begin by entering a room and are prompted with command options. Each action affects the game's state.
Available Commands:

| Command     | Description                                    |
| ----------- | ---------------------------------------------- |
| `look`      | List all visible items in the room             |
| `inventory` | Check what items you're currently carrying     |
| `go <dir>`  | Move to a new room (where `<dir>` is n/e/s/w)  |
| `pick up`   | Pick up an item from the room                  |
| `drop`      | Drop an item from your inventory into the room |
| `exits`     | Show all available exits from the current room |
| `help`      | Show help menu with commands                   |
| `quit`      | Exit the game                                  |

📁 Code Structure

.
├── Player.java       # Defines the player, inventory, and interactions
├── Room.java         # Generic room logic, including navigation and item handling
├── Utilities.java    # Helper methods for string manipulation and command reference
├── Main.java         # (To be created) Entry point of the game and room setup

⚙️ How It Works
Player Initialization: The game creates a player with a name, starting room, and an empty or pre-defined inventory.

Room Interaction: Each room contains:

    A unique name

    Items to interact with

    List of directional exits


🖼️ Screenshots / Visuals

    ![tbrpgbanner](https://github.com/user-attachments/assets/43bd9fef-2020-43d1-ac29-dcc5f56e39b1)

✅ Suggestions for images:

    ASCII map of your house layout

    Screenshot of gameplay in terminal

    Flowchart of class relationships (Player → Room → Utilities)

🧰 Technologies Used

    Java 17 (or specify version)

    Command Line Interface (CLI)

    OOP Principles (Encapsulation, Inheritance via CustomPlayer, etc.)

    Tokenizer and StringBuilder for parsing and managing state

🚀 Getting Started

To run this project on your local machine:

1. Clone this repository

    git clone https://github.com/yourusername/text-based-rpg-java.git
    cd text-based-rpg-java

2. Compile all Java files

   javac *.java

3. Run the game

  java Main


📝 Note: The Main.java file should be created to initialize your rooms and player, then loop through rooms until continuePlay is false.
Different versions of "Main" include: GameDemoSimple.java, GameVersion2.java, GameVersion3.java, and GameVersion4.java.

