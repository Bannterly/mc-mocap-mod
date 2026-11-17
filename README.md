# About
**Motion Capture** is a Minecraft mod that allows you to record and replay player movements. It is created mainly for people who want to create complex scenes in Minecraft without using real players.

It records:
- movements
- sprinting, jumping, swimming, sneaking
- swinging hands
- using items
- items in hands and armor
- states like being on fire, being invisible, or glowing
- placing, breaking and interacting with blocks
- nearby entities and riding them

After you save recording, you can create a scene, to which you can add multiple recordings or other scenes, with parameters like player name, position offset, or start delay.

CurseForge page: https://www.curseforge.com/minecraft/mc-mods/motion-capture-mod-mocap

Modrinth page: https://modrinth.com/mod/motion-capture

# How to use

- First, you need to start recording using ```/mocap recording start```. It will record all your movements or movements of a player given as an argument. 
- Then, you can stop recording using ```/mocap recording stop``` and save it with ```/mocap recording save <name>```.
- Use ```/mocap playback start <name>``` to play recording.
- You can also create scenes to which you can add multiple recordings or other scenes, with parameters like player name, position offset, or start delay.
- To create a scene use ```/mocap scenes add <scene_name>```. Then add your recording with ```/mocap scenes add_to <scene_name> <recording_name> [wait_on_start]```. More settings can be applied with playback modifiers before adding, or later with ```/mocap scenes modify <scene_name> <element> ...```.
- To play a scene use ```/mocap playback start .<scene_name>``` - put a dot before the scene name.
- By putting a dot before the name when using ```/mocap scenes add_to (...)```, you can also add scenes to other scenes.

### Commands
```
/mocap recording [...] - Recording player movements
/mocap recordings [...] - Managing recording files
/mocap scenes [...] - Creating and modifying scenes
/mocap playback [...] - Playing scenes and recordings
/mocap settings [...] - Shows and modifies settings
/mocap misc [...] - Cache, suggestions and extension commands
/mocap info - Displays information about mod
/mocap help - Displays help message
```

# Example

Simple example of one recording used 4 times in a scene with time and position offset

![](https://raw.githubusercontent.com/mt1006/mc-mocap-mod/_common/screenshots/example1.png)

One recording of climbing stairs used multiple times in a scene with start delay

![](https://raw.githubusercontent.com/mt1006/mc-mocap-mod/_common/screenshots/example2.png)
