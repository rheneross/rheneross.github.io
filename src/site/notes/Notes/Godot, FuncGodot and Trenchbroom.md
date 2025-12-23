---
{"dg-publish":true,"permalink":"/notes/godot-func-godot-and-trenchbroom/","tags":["godot","gamedev/tech"]}
---

## Useful links
https://func-godot.github.io/func_godot_docs/FuncGodot%20Manual/FuncGodot%20Manual.html

## Project structure
This is an example, and should be adapted for the need of every projects and teams.

```shell
GodotGame/
├───raw_assets/                           # .blend / .krita / .aseprite ...
├───src/                                  # The actual godot folder
│   ├───addons/
│   │   └───func_godot/
│   ├───entities/                         # One folder per entity
│   │   ├───player/  
|   │   │   ├───player.gd                 # Godot script
|   │   │   └───player.tscn               # Godot scene file
│   │   ├───door_entity/  
|   │   |   ├───door_entity.gd            # Godot script
|   │   |   ├───door_entity.tres          # FuncGodotFGDBaseClass Resource
|   │   |   └───door_entity.tscn          # Godot scene file
│   │   └───fdg.tres                      # FuncGodotFGDFile Resource
|	├───maps/                             # Trenchbroom & Godot Scene map files
│   │   ├───level1/  
|   │   │   ├───level1.tscn               # Godot scene file
|   │   │   ├───level1_map_settings.tres  # Optional FuncGodotMapSettings Resource
|   │   │   └───level1.map                # Trenchbroom map file
│   │   └───func_godot_map_settings.tres  # Global FuncGodotMapSettings Resource
│   ├───scripts/                          # Non-entity scripts
│   ├───models/                           # Exported game models in .glb format
│   ├───textures/                         # Textures
│   └───config.tres                       # TrenchBroomGameConfig Resource
└───trenchbroom/                          # FuncGodot's "Map Editor Game Path"
    └───models/                           # Exported models, added to .gitignore
```

## TrenchBroomGameConfig Resource
![Pasted image 20250218204811.png](/img/user/Notes/medias/Pasted%20image%2020250218204811.png)

## Trenchbroom Settings
Don't forget to set the game path in TrenchBroom's Settings
![Pasted image 20250218204715.png](/img/user/Notes/medias/Pasted%20image%2020250218204715.png)

## 3D models workflow
Ar the moment, my 3D models workflow is not optimal.
1. Create the model in blender, with the materials
2. Export the model as an glb to Godot
3. Create a Godot scene, with the model in it, rotate it to face the correct direction
4. Create an entity resource using the model
5. Export the entities library
6. Reload the entities in trenchbroom

In my own engine, I think I would to create a blender plugin, so I can generate the entity definition from blender, automatically if there is no script attached (Like for a prosp), and adding the script name and the properties if it's a more advanced entity.

One of the tool I will work on next week, will be a Godot tool that can generate all the props entities from a model subfolder.

1. Scan the prosp folder
2. For each model found:
  1. Generate a Godot inherited scene from a template scene
  2. Add the model to it
  3. Save the scene
  4. Create an entity resource from a template
  5. Add the created scene to the resources 
  6. Add the resource to a Props sub FDG
3. Export the props sub FDG
4. Export the main FDG (if needed)

With this tool at least, the props workflow will be fine, and as there will be less interactive entities, I believe this would be enough for this game.