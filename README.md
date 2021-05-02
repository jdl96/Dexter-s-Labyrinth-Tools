# Dexter's Labyrinth Tools

Here are some tools that will give you the ability to access the hidden in-game editor, create your own custom levels, and load custom levels into the original game without any modifications!

### Custom Levels Enabler

The Custom Levels Enabler does two things:
1. It will allow you to load a single text file that contains a levelset for the game to play when you start a new game. Loading a levelset is not permanent and will not modify the original game in any way.
2. You will be able to press a new "OK!" button on the title screen to get access to the hidden developer's level editor. This button is normally hidden outside of the game's rendering window, but I was able to move it back into view using scripting. This change is also not permanent.

#### IMPORTANT NOTES:
1. Loading custom levelsets will work with both the online and Power Play versions of the game, but attempting to use the password system in the Power Play version to access a non-existent level in a custom levelset will result in the game crashing due to a script error.
2. The "OK!" button that is used to get access to the in-game hidden editor is only available in the online 30-level version of the game. It doesn't appear in the Power Play version.
3. I recommend that you only use the hidden editor to play-test your custom levels. It does not actually have a working save function, so you will not be able to save custom levelsets using it. This is why I have created a separate editor (see below).

### Dexter's Labyrinth Editor

Created in Game Maker Studio, this new editor is meant to be used alongside the hidden developer's editor (see above). The idea is to design and play-test your levels in the developer editor, and then once you're happy with your creation, you copy the level design into this new editor in order to actually save it, since the developer's editor does not save anything for unknown reasons.

You will only be able to save one level at a time with this Editor. If you want to create a levelset that has more than one level in it, you will have to manually open the level text files in a text editor and combine them into a single file. Please refer to the `Dexter_Level_Structure_&_Values.txt` file for an example on how to structure your levelset files.

## Usage

The new Editor is self-explanatory.

To run the Custom Levels Enabler (and the game itself), you will need a [Shockwave Projector.](https://archive.org/download/ProjectorSkeletonForAdobeDirector12.0.0.111/Projector%20Skeleton%20for%20Macromedia%20Director%208.5.1.102.zip) Open the `CustomLevelsEnabler.dir` file in the Projector and use the mouse to select which option you want. Then, it will automatically try to load `Dexter's_Labyrinth.dcr` if it's in the same folder as the Enabler. If it's not found, a dialog will open where you can point the Projector to the game DCR. If you're trying to load a custom levelset, it will ask you for the levelset file first before attempting to open the game.

In this repository I have included a test levelset (consisting of two levels) and a levelset that contains 3 unused levels that were found in the original game for you to play around with.

## Level Passwords

Neither of these tools allow you to change the level passwords for the Power Play version, but for reference, here they are:
```
MOLECULE - Level 5
CALCULATOR - Level 10
EXPERIMENT - Level 15
MICROCHIP - Level 20
PROCESSOR - Level 25
MEGABYTE - Level 30
SCIENTIST - Level 35
SOFTWARE - Level 40
CIRCUITRY - Level 45
APPLICATION - Level 50
ELECTRON - Level 55
RADIATION - Level 60
DIGITIZE - Level 65
MOTHERBOARD - Level 70
PROTOCOL - Level 75
TRANSISTOR - Level 80
```

## Credits
The new Editor and most of the scripting was created by jdl.

Script for loading custom levelsets was made possible with the help of tomysshadow.
