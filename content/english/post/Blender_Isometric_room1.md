---
title: "Modeling an Isometric Room in Blender 1"
date: 2022-03-26T09:00:08+01:00
Description: ""
Tags: []
Categories: ["blog","personal","blender"]
DisableComments: false
thumbnail: "images/Blender_.png"
---
Just some notes I made while following along with this [Isometric room modeling blender tutorial](https://youtu.be/AScTgh_V4Dw).

- Notes below correspond to [this YouTube video](https://youtu.be/AScTgh_V4Dw)

- You can download a PDF copy of this post [here](www.google.com)

- You can download the associated “.blend” file [here](www.google.com). This file is the result of my work after following along with the steps in the YouTube video.

------------------------------------------
## Basic Shape Of The Room

* Create a new Blender file, select all objects and delete them.
* Add a Mesh -->> Plane with **"Shift + A"**.
* Scale it up by 4.

![Screenshot](/images/iso_room1/1.png)

* Tab to Edit Mode, go to Edge Select and select these two edges.

![Screenshot](/images/iso_room1/2.png)

* Once those two edges are selected, extrude them along the Z-axis with **"E"** by 7.
* Select all objects with **"A"**, press **"Alt + E"** to bring up the **Extrude Menu** and select **Extrude Faces Along Normals**

![Screenshot](/images/iso_room1/3.png)

* When in that mode, press **"S"** so that the extrusion should be even.

*Make it about this thick*
![Screenshot](/images/iso_room1/4.png)

* Go to Face Select, select the floor, **"Shift + D"** to duplicate it, right click to cancel movement and with **"P"** make it its own object.
* Tab back to Object Mode, select the new duplicated floor and tab to Edit Mode.

## Commencing The Floor Tile

* With the floor selected press **"Ctrl + R"** to create a loop cut, press 7 to make seven cuts and left click to validate. Right click to cancel movement.
* Do the same vertically or horizontally so that we have a grid floor pattern.

![Screenshot](/images/iso_room1/5.png)

* Select all of these faces to only leave one and delete them.

![Screenshot](/images/iso_room1/6.png)

* Press **"A"** to select the remaining tile and extrude it by however you want.
* Add an **"Array Modifier"** in the **Modifier** panel.

![Screenshot](/images/iso_room1/7.png)

* Change the **Factor X** to **-1**.
* And add the number on **Count** until it fills the floor.

![Screenshot](/images/iso_room1/8.png)

* Add another Array Modifier but change it to **0** on the X but **-1** on the Y.
* Increase the **Count** as before to fill the floor.

*Result*
![Screenshot](/images/iso_room1/9.png)

## Adding Equipments

* Change the position of the 3D-cursor with **"Shift + Right Click"** and put it on the corner of the room.
* Add a Mesh -->> Plane.
* Tab to Edit Mode with the plane selected(previously we were in Object Mode).
* Extrude it to about the height you want.

![Screenshot](/images/iso_room1/10.png)

* Put the 3D-cursor near the fridge so that we can start adding the kitchen counter.

*About there*
![Screenshot](/images/iso_room1/11.png)

**Note:** Don't forget to tab back to Object Mode before adding any new object.

* Tab back to Object Mode and add a Mesh -->> Plane.
* Scale and move it to about like this:

![Screenshot](/images/iso_room1/12.png)

* Extrude it to wherever you want.
* Select the top face, duplicate it and make it its own object.
* Tab out of Object Mode, select this new object and tab back into Edit mode.
* Extrude it.

*Result from here on*
![Screenshot](/images/iso_room1/13.png)

* Select the face on the right:

![Screenshot](/images/iso_room1/14.png)

* And drag it out along the Y-axis.

![Screenshot](/images/iso_room1/15.png)

* Tab out, select the counter and tab back in.
* Select the front face.
* Duplicate and make it its own object.
* Tab out, select this new object and tab back in(Edit Mode just in case you forget).
* Do a loop cut and cut it in half.
* Select the right most face and delete it then add a **Mirror Modifier**.
* Move all these 3 edges to make it look like this:

![Screenshot](/images/iso_room1/16.png)

* Extrude it out to about here:

![Screenshot](/images/iso_room1/17.png)

* Tab out, change the position of the 3D-cursor to here:

![Screenshot](/images/iso_room1/18.png)

* Add a Mesh -->> **UV Sphere** and reduce its topography:

![Screenshot](/images/iso_room1/19.png)

* Scale it down and move it out so that it resembles a handle.
* Add a mirror modifier and at the level of **Mirror Object**, select the counter.

![Screenshot](/images/iso_room1/20.png)

And here is what we have until now:

![Screenshot](/images/iso_room1/21.png)

* Select the top left and top right edge of the fridge.
* **"Ctrl + B"** to **Bevel**.
* With **Middle mouse button**, scroll up to add segment to make it more round or use the bevel menu:

![Screenshot](/images/iso_room1/22.png)

*Result*
![Screenshot](/images/iso_room1/23.png)

* Select the front face of the fridge, duplicate it and make it its own object.
* Tab out, select the object and tab back in.
* Extrude it.
* Deselect the bottom edge and then bevel it.

![Screenshot](/images/iso_room1/24.png)

* Select the counter and its two doors, duplicate it and move it up.

![Screenshot](/images/iso_room1/25.png)

* Move the new two doors down a bit.
* Select the whole top shelf(with its doors), go to Wireframe mode and select the whole front.

*Select these whole vertices*
![Screenshot](/images/iso_room1/26.png)

* Move it back with **"G"**.
* Now choose the bottom vertices:

![Screenshot](/images/iso_room1/27.png)

* Move them up.
* Duplicate the handles, move them up and back to also make handles for the cabinets.

![Screenshot](/images/iso_room1/28.png)

## Adding A Sink

* Move the 3D-cursor to about here:

![Screenshot](/images/iso_room1/29.png)

* Add a Cube.
* Scale it down and along the counter.

![Screenshot](/images/iso_room1/30.png)

* Duplicate it.
* Select the top of the counter without deselecting the cube.
* Press **"Shift + Ctrl + B"** to open the **Bool tool** menu.

*Choose this*
![Screenshot](/images/iso_room1/31.png)

* Now choose the duplicate cube and the main body of the counter and press **"Shift + Ctrl + B"** to open the **Bool tool** menu and choose difference.

![Screenshot](/images/iso_room1/32.png)

* Go to Wireframe mode with the original cube selected and in Edit Mode and select the bottom of the cube.

![Screenshot](/images/iso_room1/33.png)

* Press **"X"** and delete Vertices.
* Select everything with **"A"** and move it down to about here:

![Screenshot](/images/iso_room1/34.png)

* Press **"X"** and delete Only Faces.
* Now select all again and extrude it up.
* Fill the face with **"F"**.
* Extrude it out just a bit.
* Press **"I"** to **Inset**, and then extrude it down.

*Result*
![Screenshot](/images/iso_room1/35.png)

* Tab back out and in, and select this edge then press **"Shift + S"** to open this menu and choose what you are seeing:

![Screenshot](/images/iso_room1/36.png)

* Tab out into Object Mode, and add a plane.
* Scale it down.
* Tab into Edit Mode, extrude it out.
* Make a loop cut at the top and extrude that part out.

![Screenshot](/images/iso_room1/37.png)

![Screenshot](/images/iso_room1/38.png)

* Scale, move the faucet as you wish.
* Now duplicate the faucet and hold down **"Ctrl"** to snap to faces.
* Put in on the fridge and rotate it so that its like this:

![Screenshot](/images/iso_room1/39.png)

## Adding A Window

* Change the position of the 3D-cursor to the wall here:

![Screenshot](/images/iso_room1/40.png)

* Add a Cube.
* Scale it to about this much:

![Screenshot](/images/iso_room1/41.png)

* Tab into Edit Mode, select the front face, duplicate it and make it its own separate object.
* Select the original cube and **"Shift + Left Click"** to also select the room and press **"Shift + Ctrl + B"** to open the **Bool tool** menu and choose difference.

![Screenshot](/images/iso_room1/42.png)

* Move the face remaining back to about here:(should be in Edit Mode with the face selected)

![Screenshot](/images/iso_room1/43.png)

* Press **"I"** to Inset and extrude it in.

![Screenshot](/images/iso_room1/44.png)

### Styling The Window

* Add a loop cut in the middle.
* Choose the lower face and extrude it in.
* Choose the upper face, inset it and also extrude it in.

*Ta-da !! A sliding window design*
![Screenshot](/images/iso_room1/45.png)

## Adding A Table

* Change the position of the 3D-cursor to here:

![Screenshot](/images/iso_room1/46.png)

* Tab out to Object Mode, then add a plane.
* Scale it however you want.
* When done, press **"Shift + S"** and choose **Cursor to Selected**.

![Screenshot](/images/iso_room1/47.png)

* Tab into Edit Mode, move the plane up to about the window.

![Screenshot](/images/iso_room1/48.png)

* Extrude it to make it thick.

![Screenshot](/images/iso_room1/49.png)

* Tab out to Object Mode and add another plane.
* Scale it down to how you want the legs of the table to be.
* Go to top view with **7** and put it to the top right:

![Screenshot](/images/iso_room1/50.png)

* Extrude it out to make the leg thick.
* Then add a Mirror modifer and choose the table as the mirror object.
* Mirror it on both X and Y-axis.

*Result*
![Screenshot](/images/iso_room1/51.png)

We are done with the room in general. Now we want to bevel most of the things in the room but those that we don't want to bevel we must hide them:

*Hide these*
![Screenshot](/images/iso_room1/52.png)

*After hiding*
![Screenshot](/images/iso_room1/53.png)

* Select the table and add a **Bevel Modifier**.
* Change all these settings as you see:

![Screenshot](/images/iso_room1/54.png)

* Hold Left Click and pass the cursor over everything to select them all.
* Ensure the table is still selected and select this option:

![Screenshot](/images/iso_room1/55.png)

This will apply this bevel settings to everything we selected. Now click on every object and modify the bevel settings if it doesn't look right(the floor for example).

* Select everything once more, right click and **Shade Smooth**.
* Go as the image below:

*Make sure to hold **Alt** before checking Auto Smooth and changing the angle to 180°*
![Screenshot](/images/iso_room1/56.png)

* Press **"Alt + H"** to **Unhide Objects**.
* **"Shift + S"** and snap the cursor back to the world origin.
* Add a plane and scale it up.

![Screenshot](/images/iso_room1/57.png)

* Press **"N"** to bring up the right panel and there you will see **PR Isocam**.
* Click it and choose **TrueIsocam**.

![Screenshot](/images/iso_room1/58.png)

![Screenshot](/images/iso_room1/59.png)

![Screenshot](/images/iso_room1/60.png)

## Adding Material

* Press and hold **"Z"** to switch to **Material Preview**
* Click on the background and go here:

![Screenshot](/images/iso_room1/61.png)

* Add a new material and change its color.

![Screenshot](/images/iso_room1/62.png)

* Click the wall and do the same.
* Basically click on every part and change the color as you wish.