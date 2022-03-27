---
title: "Blender Basics"
date: 2022-03-13T17:15:33+01:00
Description: "Just some notes I made while following along with this basic 101 blender tutorial."
Tags: []
Categories: ["blog","personal","blender"]
DisableComments: false
thumbnail: "images/Blender_.png"
---

Just some notes I made while following along with this [basic 101 blender tutorial](https://youtu.be/9NT_1BvV2yw).

- Notes below correspond to [this YouTube video](https://youtu.be/9NT_1BvV2yw)

- You can download a PDF copy of this post [here](www.google.com)

- You can download the associated “.blend” file [here](www.google.com). This file is the result of my work after following along with the steps in the YouTube video.


# Selecting Objects

You start out in the 3D viewport.

- “A” to select all objects.
- “A A” to de-select all objects.

# Deleting Objects

When an object is selected you can delete it with:

- “Delete key” to delete the selected object.
- “X” to delete the selected object.

# Add Objects

You can add any object by hitting “Shift + A”.

# Duplicating Objects

You can duplicate an object by selecting it and hitting “Shift + D”.

# Moving Objects

- “G” to grab items and move them around.
- “X”, “Y”, and “Z” to snap to an axis and move along it.
- “Esc” or right click to cancel.
- Left click or enter to commit to the move.
- “Control + Z” to undo.
- “Shift + Control + Z” to redo.

Alternatively, you can use “Middle Click and Hold” to change axis. This will let you choose on which axis to move the object then you can leT go and continue moving it on that axis.

# Rotating Objects

- “R” to rotate items.
- “R R” to go to track ball rotation.
- “X”, “Y”, and “Z” to snap to an axis and rotate along it.
- “Esc” or right click to cancel.
- Left click or enter to commit to the move.
- “Control + Z” to undo.
- “Shift + Control + Z” to redo.

Alternatively, you can use “Middle Click and Hold” to change axis of rotation as previously mentioned.

# Scaling Objects

- “S” to scale.
- Global by default (scales equally in all directions).
- “X”, “Y”, or “Z” to choose an axis to scale along.
- “Esc” or right click to cancel.
- “Shift + Control + Z” to redo.

Alternatively, you can use “Middle Click and Hold” to change axis of scaling as previously mentioned.

# Hide Objedcts

- “H” to hide object.
- “Alt + H” to un-hide object.

# Changing Your Viewpoint

### Orbiting

There are **four ways** to orbit (move around a point in the 3D viewport):

1. When using a 3-button mouse, orbit by clicking and holding the middle mouse button while moving the mouse.
1. With a 2-button mouse or standard laptop trackpad, turn on “Emulate 3-button Mouse” from the settings, then hold down “Alt” while moving the mouse or touching the trackpad:

![Screenshot](/images/blender/screenshot_1.png)

![Screenshot](/images/blender/screenshot_2.png)

**A note for Mac users:** You might want to use the “Command” key (“OS Key”) instead of “Alt”.

3. On a multitouch trackpad (like the one on a MacBook), use two fingers to orbit.
4. Use the orbit tool in the upper left-hand corner of the 3D viewport:

![Screenshot](/images/blender/screenshot_3.png)


### Panning

There are **four ways** to pan:

1. Hold down “Shift” + middle mouse button on your mouse.
2. On a multitouch trackpad, “Shift” + two fingers on the trackpad to move.
3. On an ordinary trackpad, “Shift + Alt” (Emulate 3 button mouse) + one finger on the trackpad to move.
4. Use the pan tool:

![Screenshot](/images/blender/screenshot_4.png)

### Zooming

1. With a mouse, use the scroll wheel to zoom in and out.
    - For a “smoother” zoom, use “Control” + middle mouse button.
2. On a multitouch trackpad, use two finger “pinch and zoom” to zoom in and out.
3. On an ordinary trackpad, simulate middle mouse button with “Alt” to zoom.
4. Use the zoom tool:

![Screenshot](/images/blender/screenshot_5.png)

### Focusing On An Object

You can also switch to viewing a particular object by first selecting the object, then hitting the “.” (period) key on the number pad.

If you are on a laptop and don’t have a full size keyboard with a number pad, then use the tilde “~” key while the object is selected, which will open up a view menu on top of the object. From that menu, select “View Selected” or hit “3” on your keyboard:

![Screenshot](/images/blender/screenshot_6.png)

Also, you can use “Shift + B”, then *drag over area* to center the view on the object dragged on.

### Align With A Particular Axis(X, Y, Z)

There are several ways to align the viewport to a particular axis. The first is to use the orbiter tool (click on one of the three letters, “X”, “Y” or “Z”) on the orbiter tool:

![Screenshot](/images/blender/screenshot_7.png)

**Or better, just learn the keyboard shortcuts**

- Use the “1” key for front view.
- Use the “3” key for side view.
- Use the “7” key for top view.

On a laptop or keyboard without a number pad, you will have to enable **Number Pad Emulation** first from Edit –> Preferences –> Input:

![Screenshot](/images/blender/screenshot_8.png)

By default, aligning to an axis turns on **orthographic mode** (meaning objects are shown with no sense of perspective). This is good when editing and aligning things, but may not be so great when you are trying to get a sense for how your scene looks overall. You can toggle this on and off using “5” on your number pad (or just the “5” key along the top of your keyboard, if you’ve turned on number pad emulation).

Here’s the view with orthographic mode turned on:

![Screenshot](/images/blender/screenshot_9.png)

Versus with orthographic mode turned off:

![Screenshot](/images/blender/screenshot_10.png)

If you look closely at the second picture, you’ll notice the grid lines are heading towards a vanishing point somewhere farther back in the scene (i.e. there is a sense of perspective).

### Other Ways To Align To View

- From View -> Viewport on the top menu bar in blender.
- Using tilde “~” while an object is selected, to open the view menu.
- Alt + middle mouse button while orbiting will snap the view to each axis as you orbit.

### Move 3D Cursor

Use "Shift + Right Click" to move the 3D Cursor on the 3D Viewport.

# Dealing With Blender If You Are Used To Other 3D Software

Under settings, you can use a more standard key map by going to: Edit -> Preferences - Key map and choosing **Industry-standard Key map.**

![Screenshot](/images/blender/screenshot_11.png)

# Object And Scene Properties

## Object Properties

The right-hand side of the viewport will show properties of objects (i.e. material properties such as color, surface type, object dimensions, etc…):

![Screenshot](/images/blender/screenshot_12.png)

## Scene “Collection”

The “Collection” is an organized view of all the items in the scene (objects, cameras, lights, etc…):

![Screenshot](/images/blender/screenshot_13.png)


## Viewing Your Scene From The Camera

When you render a scene in Blender, the render is performed from the perspective of the camera. There are four different ways to see what your camera is seeing:

1. Number pad + “0” (Zero), or “Fn + 0” (function key + zero) if you’re on a Mac.
2. The camera icon on the right-hand side of the screen:

![Screenshot](/images/blender/screenshot_14.png)

3. View -> Viewport -> Camera from the top menu bar.
4. Tilde “~”, then choose “Camera View”.

# Toggle Panels

- “T” to toggle on or off the Left Panel.
- “N” to toggle on or off the Right Panel.