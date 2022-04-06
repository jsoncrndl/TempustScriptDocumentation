---
title: Walk and Run Commands
tags: [walk, run, move, position]
keywords:
summary: "Make an object move to a location over time"
sidebar: tempustscript_sidebar
permalink: move.html
folder: tempustscript
---

# The "walk" and "run" Commands

The walk and run commands are used to move an object slowly over time. They generally accomplish the same task, only changing the speed of the movement. To set the position of an object instantly, use the [setpos](setpos.md) command.

**Usage**

    move [object] to [coords]

The object argument can be omitted, and it will target "obj". For information on objects, see [here.](objects.md)

For information on coordinates, see [here.](objectcoords.md)

## Example

    move to y:obj-1
    say["???"] "Please excuse me..."
    move plr to x:plr+1
    move to y:obj-10
    disable obj

## Unity Implementation

There are several ways to move a character in Unity. The default implementation simply moves the transform of the object, since this will work regardless of the components attached to the object.

To customize the implementation, override the OnWalk() and OnRun() methods in the TSManager. It is a good idea to override this to use your game-specific method of moving a character and include any movement animations.
