# obj-importer-for-sledding-game-BETA-NO-TEXTURES-YET-OBJ-HAS-TO-BE-CALLED-MODEL-.OBJ
Cessna Importer for MelonLoader
Version: 2.2.0

Developer: Scott

Overview
The Cessna Importer is a powerful utility mod designed to dynamically bridge external 3D assets into the game environment. Built specifically for games running the Il2Cpp runtime with MelonLoader, this mod allows users to bypass hardcoded asset limitations by importing raw .obj models and .png textures directly into a live game session.

Key Features
In-Game Mod Menu: Toggle a clean, functional UI using the [Insert] key to manage imports without restarting the game.

Dynamic Asset Loading: Point the mod to any local folder to instantly spawn your model with its associated texture.

Advanced Rendering Fix: Includes a specialized Visibility Fix that "steals" the game's native shaders. This ensures that imported models respect the game's lighting and environment (such as snow or fog) instead of appearing purple or invisible.

Automatic Mesh Optimization: The importer automatically recalculates normals, bounds, and handles missing UV maps to ensure the model looks correct under any lighting condition.

Collision Support: Automatically generates a MeshCollider based on the imported geometry, allowing your model to have physical presence in the world.

How to Use
Preparation: Place your 3D model (named model.obj) and your texture (named texture.png) into a folder of your choice.

Launch: Start the game with MelonLoader installed.

Open Menu: Press the [Insert] key to open the importer menu.

Path Input: Copy and paste the folder path into the text field.

Import: Click "Import & Apply Visibility Fix". The model will spawn 7 units in front of your character.

Technical Specifications
Requirement: MelonLoader 0.6.0+

Compatibility: Universal Il2Cpp Support

Shader Logic: Forces Opaque rendering with ZWrite enabled and alpha-blend keywords disabled to prevent transparency artifacts common in modded Unity imports.
