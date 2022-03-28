---
title: "Blender Donut Notes: 01"
date: 2022-03-28T18:11:59+01:00
Description: ""
Tags: []
Categories: ["blog","personal","blender"]
DisableComments: false
thumbnail: "images/Blender_.png"
---
Just some notes I made while following along with this [now famous blender donut tutorial](https://www.youtube.com/watch?v=nIoXOplUvAw&list=PLjEaoINr3zgFX8ZsChQVQsuDSjEqdWMAD&index=1).
- Notes below correspond to [this YouTube video](https://youtu.be/imdYIdv8F4w?list=PLjEaoINr3zgFX8ZsChQVQsuDSjEqdWMAD)
- You can download a PDF copy of this post [here](www.google.com)
- You can download the associated “.blend” file [here](www.google.com). This file is the result of my work after following along with the steps in the YouTube video.

## Adding A New Object

* Add new objects with **“Shift + A”**.
* Try to choose an object that is as close to the finished shape you’re shooting for as possible (in this case, a torus is pretty close to a donut):

When you add a new shape, a menu will come up at the bottom that allows you to edit the shape’s properties. If you accidentally close this menu, you can bring it back up with **“F9”**:

![Screenshot](/images/Blender_donut1/1.png)

> ***Tip:*** *When setting the number of “Major segments” and “Minor segments” for the torus, keep the numbers relatively low. Making things high resolution at the start of a project is more work for blender and more work for you, since you will be stuck editing object meshes that have a huge number of faces and vertices.*

You should also try to choose a number of major and minor segments that results in relatively square faces on the surface of the object, like this:

![Screenshot](/images/Blender_donut1/2.png)

## Scaling

It’s important to keep things as close as possible to their real-life scale. The donut above has a radius of about **one meter**, so it’s enormous. Use the **“S”** key to scale down to a more appropriate size. Say, 0.1 meters (10 centimeters) for a start.

Hitting the **“N”** key will bring out a side menu like the one shown here. You’ll see that the scale of the object is now around “0.033”. You pretty much always want this to be **“1**”. We can “apply” our object’s new scale with **“Control + A”**, then choose **“Scale”** from the menu that pops up, as shown here:

![Screenshot](/images/Blender_donut1/3.png)

## Shading

Blender has two types of object shading: *flat* and *smooth*. Our donut looks “blocky” because by default blender uses flat shading. If we right-click on the donut and choose **“Shade smooth”**, blender will switch to using smooth shading:

![Screenshot](/images/Blender_donut1/4.png)

Which gives us a much nicer-looking result:

![Screenshot](/images/Blender_donut1/5.png)

**Note:** Shade smooth doesn’t “add any geometry”. It simply makes the object appear smooth in the viewport. We can make the object actually smoother using a “sub surf” operation:

![Screenshot](/images/Blender_donut1/6.png)

![Screenshot](/images/Blender_donut1/7.png)

## Editing

> ***Tip:*** *To switch into **Edit Mode**, hit the “Tab” key. Edit mode allows you to edit the object’s mesh (“skeleton”).*

Edit mode looks like this:

![Screenshot](/images/Blender_donut1/8.png)

Clicking on a face or a vertex allows you to modify it. We can (for instance) grab a vertex and then drag it away from the donut:

![Screenshot](/images/Blender_donut1/9.png)

> ***Tip:*** *Hold down “Shift” to select multiple points (vertices).*

A better way to change shapes is to enable proportional editing which will automatically grab vertices around your selected vertex, and will modify them as a group. Like this:

![Screenshot](/images/Blender_donut1/10.png)

Notice the circle in the screenshot above: this is the area-of-effect for proportional editing.

You might not be able to see the circle (the default area-of-effect is far, far larger than the donut). You can use the *scroll wheel* to scroll up, which will reduce the area-of-effect until you can see it.

If you are on a laptop, you can first:

1. Select a vertex on the donut.
1. Left-click once.
1. A “Move” menu will show up in the bottom left hand corner of the screen (see the screenshot above).
1. Open that menu, and change the proportional scale to something reasonable (say 0.04 or 0.05), at which point you should be able to see a little gray ring as in the screenshot above.
1. On a multitouch trackpad, use two fingers to scale the ring in and out to control the area-of-effect.

Note, you can also turn proportional editing on and off from a “Move” menu that appears in the lower-left when grabbing a part of the mesh:

![Screenshot](/images/Blender_donut1/11.png)

## The "Shrink And Flatten" Tool

Rather than grabbing a vertex and moving it away from the surface of the donut, **“Alt + S”** (“Fn + S” on a mac) will open the “shrink and fatten” tool, which will move faces towards (or away) from the surface of the donut based on their direction (in other 3D software, this is called “move along normals” or something similar).

## Select Random

You can also select vertices on your shape entirely at random, like this:

![Screenshot](/images/Blender_donut1/12.png)

![Screenshot](/images/Blender_donut1/13.png)

This can be used to add some random imperfections to the donut. Grab the randomly selected vertices and move them in or out from the donut for a bumpy effect!