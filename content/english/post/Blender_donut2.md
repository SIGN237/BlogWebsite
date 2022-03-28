---
title: "Blender Donut Notes: 02"
date: 2022-03-28T18:40:40+01:00
Description: ""
Tags: []
Categories: ["blog","personal","blender"]
DisableComments: false
thumbnail: "images/Blender_.png"
---
Just some notes I made while following along with this [now famous blender donut tutorial](https://www.youtube.com/watch?v=nIoXOplUvAw&list=PLjEaoINr3zgFX8ZsChQVQsuDSjEqdWMAD&index=1).
- Notes below correspond to [this YouTube video](https://youtu.be/7wKnPclzYY8?list=PLjEaoINr3zgFX8ZsChQVQsuDSjEqdWMAD)
- You can download a PDF copy of this post [here](www.google.com)
- You can download the associated “.blend” file [here](www.google.com). This file is the result of my work after following along with the steps in the YouTube video.

## Selecting Things In Edit Mode

We need to select the top of our donut (we will duplicate this and make it thicker: it will be our icing).

To do this, from edit mode select “X-Ray mode”, which will make the donut appear “see through”:

![Screenshot](/images/Blender_donut2/1.png)

When we select things in X-Ray mode, we can be sure we’re selecting all the way “through” the object (i.e. vertices on the other side of the object will also be selected). Also, make sure you’re looking at the object directly ON, say from the X or Y axis (as above).

## Duplicate

Duplicate the top half of the donut by selecting it and hitting “Shift + D”. This will make a copy of the selected part of the mesh and lock it to your cursor:

![Screenshot](/images/Blender_donut2/2.png)

We want the mesh right on top of its original position, so we can hit **“Esc”** to put it back where it belongs:

![Screenshot](/images/Blender_donut2/3.png)

Next, we hit the **“P”** key and choose **“Selection”**, to convert our duplicated mesh into its own object:

![Screenshot](/images/Blender_donut2/4.png)

If we cancel out of Edit Mode and return to the object viewer by hitting **“Tab”**, we’ll see two objects (as indicated by the outlines in two different colors):

**Helpful tip:** You can double-click on things in the layer editor at the upper right-hand corner, to rename them. Here, I have renamed my two objects to **“Donut”** and **“Icing”**:

![Screenshot](/images/Blender_donut2/5.png)

**Another good tip:** If you accidentally clicked away from your selection before hitting **“P”** to make your mesh into a separate object, you can also hit **“Control + L”** to select the **“linked”** vertices that make up your icing, then you can hit “p” to separate it.

You can also rename by hitting **“F2”** while you have one of your object selected in the object viewer.

Next, add a **“Solidify”** modifier to the icing:

![Screenshot](/images/Blender_donut2/6.png)

Then, choose Wireframe Mode, so you can see through the wire mesh:

![Screenshot](/images/Blender_donut2/7.png)

## Dealing With Inverted Normals 

You might find that when changing the offset to a positive value, the icing layer appears to be thickening **into** the donut rather than outwards. This is because the “normals” for the icing are facing the wrong way (i.e. they are facing into the donut).

You can check this by entering edit mode, then turning on “Face Orientation” from **“Viewport Overlays”:**

![Screenshot](/images/Blender_donut2/8.png)

You can flip the normals from the “Mesh” menu near the top of the screen, like so:

![Screenshot](/images/Blender_donut2/9.png)

Afterwards, the color of the mesh should change:

![Screenshot](/images/Blender_donut2/10.png)

This should fix any issues with the icing appearing to “offset” into the donut when the **“Solidify”** modifier is applied.

If the icing *still* looks funny, try changing the order of the modifiers, so that solidify is applied first:

![Screenshot](/images/Blender_donut2/11.png)

