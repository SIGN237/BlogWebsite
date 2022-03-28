---
title: "Blender Donut Notes: 03"
date: 2022-03-28T18:56:24+01:00
Description: ""
Tags: []
Categories: ["blog","personal","blender"]
DisableComments: false
thumbnail: "images/Blender_.png"
---
Just some notes I made while following along with this [now famous blender donut tutorial](https://www.youtube.com/watch?v=nIoXOplUvAw&list=PLjEaoINr3zgFX8ZsChQVQsuDSjEqdWMAD&index=1).
- Notes below correspond to [this YouTube video](https://youtu.be/R1isb0x4zYw?list=PLjEaoINr3zgFX8ZsChQVQsuDSjEqdWMAD)
- You can download a PDF copy of this post [here](www.google.com)
- You can download the associated “.blend” file [here](www.google.com). This file is the result of my work after following along with the steps in the YouTube video.

## Hiding Modifiers

We want to hide the solidify modifier we added to the icing, so that it doesn’t cover up our mesh while we’re in edit mode (otherwise, it’s quite hard to edit the mesh since we can’t select it).

With solidify turned on in the viewport, edit mode for our icing looks like this:

![Screenshot](/images/Blender_donut3/1.png)

With solidify turned off in the viewport, we see this (much better!):

![Screenshot](/images/Blender_donut3/2.png)

## Snapping Our Icing To The Face Of The Donut

We now want to give our icing some “dribbly bits” that droop down the donut (like real icing tends to do as it cools). From edit mode, if we grab a vertex on the icing mesh and simply drag it down (with proportional editing turned on), the rest of the mesh will tend to end up “inside” the donut, like this:

![Screenshot](/images/Blender_donut3/3.png)

You can fix this using the **“Snap”** tool at the top of the viewport. Make sure you select **“Snap to Face”** and **“Project Individual Elements”**, as shown here:

![Screenshot](/images/Blender_donut3/4.png)

Dragging the mesh now keeps the icing snapped to the surface of the donut:

![Screenshot](/images/Blender_donut3/5.png)

> ***Note:*** *The option “Project Individual Elements” in the snap tool is actually what causes all of our selection to snap to the surface of the donut, rather than just the single vertex we selected.*

## Adding A Reference Image

It’s always a good idea to “work from reference”, so go find a donut that you like.

In my case, I am using a freely available image from the Wikimedia Commons. Here’s[a link to that image](https://commons.wikimedia.org/wiki/File:Dunkin-Donuts-Chocolate-Sprinkled.jpg).  I reproduce it here as well:

![Screenshot](/images/Blender_donut3/6.jpeg)

We can pull this image into Blender for use as a reference. We can do this by “splitting” the viewport.

First, place your cursor on the border between two windows in the viewport:

![Screenshot](/images/Blender_donut3/7.png)

Then choose **“Vertical Split”**:

![Screenshot](/images/Blender_donut3/8.png)

Drag the new window into place, until it is as wide (or narrow) as you feel is appropriate:

![Screenshot](/images/Blender_donut3/9.png)

Now, we switch the new window to **“Image Editor”**, and pull in our donut:

![Screenshot](/images/Blender_donut3/10.png)

![Screenshot](/images/Blender_donut3/11.png)

![Screenshot](/images/Blender_donut3/12.png)

> ***Note:*** *Images pulled into blender in this way do not become part of your **.blend** file, so if you move the image, you’ll have to re-import it!*

## Shape The Icing

Now we can start shaping the icing to match our reference image. Before we do this, we want to apply our **“Subsurface”** modifier to the icing to increase the level of detail in the grid. Do this by moving **“Subsurface”** to the top of the modifiers list and hitting **“Control + A”** (or “Command + A” on a Mac) to apply it. In edit mode, the icing mesh should now appear to have more faces than before:

![Screenshot](/images/Blender_donut3/13.png)

![Screenshot](/images/Blender_donut3/14.png)

> ***Tip:*** *From time to time you might want to hide stuff. You can do this by selecting an object and hitting ***“H”***. ***“Control + H”*** will un-hide.*

We can now shape the icing by grabbing and dragging. We can also make small “drippy” bits by selecting one two or more vertices and hitting **“E”** to extrude:

![Screenshot](/images/Blender_donut3/15.png)

You can rotate and scale the extruded sections with the usual **“R”** and **“S”**.

Here, I do my best to get my donut to match the reference image a bit better (I actually deleted my icing and started over with a “smaller” icing, created by selecting a smaller section at the top of my donut, to better match my reference):

![Screenshot](/images/Blender_donut3/16.png)

I now have a nice “bumpy” donut that is a rough match to my reference image. Some parts of the icing don’t seem to be properly “shaped” to the surface of the donut, though. We’ll fix that in the next step.

## Changing The Shape Of The Donut

You’ll notice that a lot of donuts have a section near their middle that is “less cooked” than the rest of the donut. This part has a lighter color, and usually forms a sort of “indent” around the center of the donut.

Hitting **“1”** to go into front view, turning on X-ray mode, and then selecting the middle portion of the donut mesh and hitting **“S”** will let you scale the mesh **in** to create this effect.

**Note:** Screenshots below were taken without this modification, so if the donut still appears “fat around the middle”, that’s why!

## The “Shrink Wrap” Modifier

Once you shrink the center of your donut, you’ll notice that the icing no longer hugs the surface of the donut. We can force the icing to adhere to the donut using the **“Shrinkwrap”** modifier.

With the icing selected, go to the modifiers pane and add a **“Shrinkwrap”** modifier:

![Screenshot](/images/Blender_donut3/17.png)

You’ll need to click on the little “eye dropper” and select the donut (the object we want to “shrink wrap” on to):

![Screenshot](/images/Blender_donut3/18.png)

Next, change the order of the icing modifiers so **“Shrinkwrap”** comes first, which will get rid of this weird “patterning” that appears:

![Screenshot](/images/Blender_donut3/19.png)

> ***Tip:*** *Weird display artifacts are usually a sign that you need to change the order of your modifiers!*