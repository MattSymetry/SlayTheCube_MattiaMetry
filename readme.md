# Slay the Cube - Task Implementation | Mattia Metry

## Overview

This repository contains the implementations for the tasks provided by PEC Game Development GmbH as part of the application process for the position of Game Developer. I implemented most tasks, even some art ones, but I do focus on and apply for the programming role. 

## Task List

### 1. Task 1: Create New Cards and Actions (Logic + Programming C#)
- **Functionality:** 
  - Implemented a new action "gassed," a status effect that causes damage over time based on accumulated poison. (And some extras, mentioned below)
  - Created a set of new cards that utilize this action, along with a special keyword.
- **Cards Implemented:**
  - Compressed Air Gas Attack (gassed action)
  - Toxic Gas Container (gassed action)
  - Amplification of Poisonous Gas (new AmplifyGas action implemented)
  - Toxic Compressor (new CompressToxic action implemented)
  - Container Creation (new ContainerCreation action implemented)
- **Remarks:**
  - All new actions are fully implemented and functional
  - All status and special keywords added.
  - All cards are added to the game and can be drawn and played accorsingly.

### 2. Task 2: Create Art Assets (Art and Creativity)
- **Functionality:** 
  - Created new images for the cards, a start screen, a map, and various characters and objects using AI tool (https://perchance.org/ai-pixel-art-generator) I mainly used the 'Fantasy Painting' art style.
- **Assets Created:**
  - Card images based on the names and descriptions.
  - Title screen with a floating cube.
  - 2D map with rooms
  - Main character (Knight)
  - Miscellaneous - only 2:
    - Well
    - Staircase
- **Remarks:**
  - I don't focus on art / apply for art, I just wanted to add something so it's not all blank :)

### 3. Task 3: Integrate Cards and Art into the Game (Logic and Programming)
- **Functionality:** 
  - Replaced the title screen and menu with newly created graphics. Small animations using code for prototype.
  - Integrated the cards into the game and visualized them.
  - Replaced rooms with placeholder assets and implemented the adjacentcy logic.
- **Events Implemented:**
  - Random event triggers upon room selection (combat, boss fight, or miscellaneous events). Created a 'Prefabs/Core/RoomManager'. On it, the chances can be set for each event (currently: comabt 60%, boss fight 10%, miscellaneous 30%)
  - For the miscellaneous events, I chose a ScriptableObjects approach as the cards etc. also do.
    - To create a new one:
        1. Open the 'Scripts/Miscellaneous/MiscellaneousData' ScriptableObject and add the new 'FunctionType' enume, the function that should be called and add it to the switch-case in 'InvokeFunction()'.
        2. Create a new miscellaneous object in 'Data/Miscellaneous'. Here you can add the description, image and choose whch function will get called based on the enum.
  - New boss has been added, but without any of the custom functionalities.
- **Remarks:**
  - Title screen and graphics integrated. (Not in any artistic way, only functionally)
  - Map navigation and event triggers functioning.
  - Events programmed and integrated. (Only 2, but easy to extend system in place)
  - New boss and added to the game. (Without custom functions)


## This is addition to the Apache Licenses:
- The submitted data, codes, type which are submitted within these tasks are the intellectual property of PEC Game Development GmbH.
- All applicants agree to these supplemental license agreements when applying for the open job postings at PEC Game Development GmbH with the corresponding codes, art and the entire repository.


