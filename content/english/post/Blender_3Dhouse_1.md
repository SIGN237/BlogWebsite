---
title: "Blender_3Dhouse_1"
date: 2022-03-15T09:34:32+01:00
Description: "Just some notes I made while following along with this 3D modeling house blender tutorial series."
Tags: []
Categories: ["blog","personal","blender"]
DisableComments: false
thumbnail: "images/Blender_.png"
---
Just some notes I made while following along with this [3D modeling house blender tutorial series](https://youtu.be/Np1kscimD4w).

- Notes below correspond to [this YouTube video](https://youtu.be/Np1kscimD4w)

- You can download a PDF copy of this post [here](www.google.com)

- You can download the associated “.blend” file [here](www.google.com). This file is the result of my work after following along with the steps in the YouTube video.

# Adding A Cube

After deleting all the objects on the scene by pressing "A" to select all, then "X" to confirm.
- **“Shift + A”** to open **Add Menu** and choose Mesh --->> Cube.

![Screenshot](/images/3D_house_tuto1/1.png)

# Object Mode Vs Edit Mode

To switch between Object and Edit mode simply press **“Tab”**.

- *Object Mode*

![Screenshot](/images/3D_house_tuto1/2.png)

- *Edit Mode*

![Screenshot](/images/3D_house_tuto1/3.png)

# Selecting Vertices, Edges and Faces in Edit mode

When in Edit Mode, the default selection is on Vertices(Vertex select).

- *Vertex Select* (we can see a vertex is selected and it is highlighted in white).

![Screenshot](/images/3D_house_tuto1/4.png)

- *Edge Select* (we can see an edge highlighted in white meaning it is selected).

![Screenshot](/images/3D_house_tuto1/5.png)


- *Face Select* (we can see a face highlighted in orange meaning it is selected).

![Screenshot](/images/3D_house_tuto1/6.png)


**Note:** To select multiple vertices, edges or faces, **“Shift + Click”** to begin selecting multiples.

# Cutting Cube In Half

To cut the cube in half we first go to the front view by pressing "1" and add a **Loop Cut** by pressing **"CTRL + R"**.
Once that's done you choose the orientation of the cut. Either horizontally or vertically.

- *Vertically*

![Screenshot](/images/3D_house_tuto1/7.png)

- *Horizontally*

![Screenshot](/images/3D_house_tuto1/8.png)

Select the face to be deleted and press **"X"** to delete then choose **"Vertices"** to delete half of the cube.

- *Before*

![Screenshot](/images/3D_house_tuto1/9.png)

- *After*

![Screenshot](/images/3D_house_tuto1/10.png)

## Mirroring The Cube

Go back to Object Mode by pressing **"Tab"** and choose **Modifier Properties** on the right:

![Screenshot](/images/3D_house_tuto1/11.png)

Choose the **Mirror** modifier on the dropdown menu:

![Screenshot](/images/3D_house_tuto1/12.png)

When this is done, you can select all objects on the scene with **"A"** and press **"G"** to move it:

![Screenshot](/images/3D_house_tuto1/13.png)

We can clearly see the mirrored side is not attached to the original one and to change this we need to check the **Clipping** property in the **Mirror modifier** properties:

- *Off*

![Screenshot](/images/3D_house_tuto1/15.png)
![Screenshot](/images/3D_house_tuto1/13.png)

- *On*

![Screenshot](/images/3D_house_tuto1/16.png)
![Screenshot](/images/3D_house_tuto1/14.png)
![Screenshot](/images/3D_house_tuto1/17.png)

# Modeling The House

* Go to **Vertex select** mode and select the two top middle vertices.
* Go to the front view by pressing **"1"**.
* Press **"G"** then **"Z"** to move these vertices along the Z-axis.
* This is to form the roof of the house.

*The two vertices selected*
![Screenshot](/images/3D_house_tuto1/18.png)

*Front view moving the vertices along the Z-axis*
![Screenshot](/images/3D_house_tuto1/19.png)

Drag and drop wherever you want by left mouse clicking. This already gives us the basic shape of the house.

By pressing and holding **"Z"** in **Edit Mode**, you will be prompted to select between 4 different views.

![Screenshot](/images/3D_house_tuto1/20.png)

Hold **"Z"** and move the cursor over any of them to select that view. Take your time and see what each of them does.

Choose the **Wireframe** mode, go back to front view by pressing **"1"** and select the front of the box by clicking and dragging *or* with **Box select** (by pressing **"B"** to access it)

![Screenshot](/images/3D_house_tuto1/21.png)

Now everything is selected both in the front and in the back. This is because *Wireframe* mode acts as an x-ray vision whereas if we were in Solid mode, only the front would have been selected.

![Screenshot](/images/3D_house_tuto1/22.png)

While everything is still selected, go back to front view with "1" and press **"G"** then **"Z"** to move the whole shape down by however you want. Left click to confirm selection.

![Screenshot](/images/3D_house_tuto1/23.png)

Go back to Solid mode by holding **"Z"** and moving the cursor to the solid mode. You can now move the camera by clicking and holding middle mouse button to see what we have.

## Adding A Door

Add two loop cuts by pressing **"Ctrl + R"** as seen below:

![Screenshot](/images/3D_house_tuto1/24.png)

![Screenshot](/images/3D_house_tuto1/25.png)

![Screenshot](/images/3D_house_tuto1/26.png)

To make the loop cut not slanted we press **"S"** to change the size and then **"Z"** to move on the Z-axis. When in this mode you can type in any value to affect the edge by it. So we type **0** and press enter to confirm our choice.

![Screenshot](/images/3D_house_tuto1/27.png)

Choose **Face Select** at the top left and select the face of the door. Press **"X"** to delete and choose *Faces*.

![Screenshot](/images/3D_house_tuto1/28.png)

## Changing The Height Of The Door

To start changing the size of the door, we need to select the whole loop of edges just above the door.

*All these edges plus some behind.*
![Screenshot](/images/3D_house_tuto1/29.png)

We can **"Shift + Click"** when in Edge select to select all of them but an easier way is to press **"Alt + Click"*** and it will select the loop. Meaning all of the edges connected.

*Don't forget to add this edge*
![Screenshot](/images/3D_house_tuto1/30.png)

Press **"G"** and then **"Z"** to move the whole loop on the Z-axis. Choose where you want the new height of the door at and left click to validate.

## Changing The Length Of The Door

If you want to change the size of the door by it's length, you will need to choose the appropriate loop to do so.

*Alt + Click to select the whole loop*
![Screenshot](/images/3D_house_tuto1/31.png)

Selecting this loop and pressing **"G"** and **"X"** to select the X-axis will move all the edge along and form like a barn shape.

*Barn shaped*
![Screenshot](/images/3D_house_tuto1/32.png)

To prevent this, we press **"G G"** to enter **Edge Slide** mode and now when moving the loop edge along the X-axis it will slide along the edge as seen below.

*The length enlarging but without giving that barn shape*
![Screenshot](/images/3D_house_tuto1/33.png)

## Applying A Modifier

Before starting to add a window, let's apply our Mirror modifier we have but for that we need to change from Edit to Object Mode by pressing **"Tab"**.
When in Object Mode, press **"Ctrl + A"** over the modifier tab to apply any modifier active.

*Mirror modifier applied*
![Screenshot](/images/3D_house_tuto1/34.png)

## Making A Window

Change back to Edit Mode to prepare to add the windows. Same as the door we add loop cuts to form the shape of the window. Press **"Ctrl + R"** and make the shape of the window.

*Loop Cut 1*
![Screenshot](/images/3D_house_tuto1/35.png)

*Loop Cut 2*
![Screenshot](/images/3D_house_tuto1/36.png)

*Loop Cut 3*
![Screenshot](/images/3D_house_tuto1/37.png)

*Loop Cut 4*
![Screenshot](/images/3D_house_tuto1/38.png)

Choose **Face Select** at the top left and select the face of the window. Press **"X"** to delete and choose *Faces*.

![Screenshot](/images/3D_house_tuto1/39.png)

Repeat the same steps and add a window at the side of the house.

*Result*
![Screenshot](/images/3D_house_tuto1/40.png)

## Making A Roof

Press **"1"** to go to front view, hold **"Z"** and pass the cursor onto wireframe to change to Wireframe Mode, and press **"C"** to enter **Circle Select** mode (another type of select). In Circle Select mode, scrolling up or down with the scroll wheel will increase or decrease the radius of the circle and clicking and dragging with left click will select. Also, holding down middle mouse click and dragging will deselect anything selected. To exit this mode you simply right click.
Now since everything is clear, go to front view and also *Wireframe* mode and select the top of the house.

![Screenshot](/images/3D_house_tuto1/41.png)

![Screenshot](/images/3D_house_tuto1/42.png)

Press and hold **"Z"** to go back to solid mode. With this top of the house selected we want to duplicate it. To do so we simply press **"Shift + D"** to duplicate select. Once it's duplicated the new object will be in move mode so press **"Z"** to move it along the Z-axis and left click to drop it anywhere.

*Roof duplicated*
![Screenshot](/images/3D_house_tuto1/43.png)

Now we want to make this new roof its own object. To do so we press **"P"** to prompt the **Separate** menu and here choose *"Selection"* to separate our new roof into a its own object.

![Screenshot](/images/3D_house_tuto1/44.png)

Go to front view with **"1"**, *Wireframe* mode with **"Z"** and move the new roof down almost at the same level as the previous roof.

*Something like this*
![Screenshot](/images/3D_house_tuto1/45.png)

### Getting Rid Of Extra Vertices On Our Roof

To get rid of extra vertices on an object, press **"Alt + Click"** to select a loop, **"G G"** to **Edge Slide** and edge slide this edge into the one nearby. When done, select the whole roof/object and press **"M"** to **Merge** our fusioned vertices and select ***By Distance***. (you should be in either Vertice or Edge select mode)

![Screenshot](/images/3D_house_tuto1/46.png)

Repeat this process until the roof is clean of any vertices.

![Screenshot](/images/3D_house_tuto1/47.png)

## Finishing Our Roof

Our roof is clean of vertices so we can go to front view with **"1"**, move it along the Z-axis with **"G"** then **"Z"** and bring it into the house just a little bit.

![Screenshot](/images/3D_house_tuto1/48.png)

Press **"S"** to scale it until it peeks out.

*Approximately like this*
![Screenshot](/images/3D_house_tuto1/49.png)

**"G"** and **"Z"** to move it down again and left click to validate.

![Screenshot](/images/3D_house_tuto1/50.png)

![Screenshot](/images/3D_house_tuto1/51.png)

Our roof is almost complete but it lacks some thickness. So to add thickness to it we press **"E"** for **Extrude** to extrude the roof and do it however thick you want.

![Screenshot](/images/3D_house_tuto1/52.png)

# Adding A Chimney

To begin adding the chimney we need to move the 3D-cursor where we want the chimney to be located. For a reminder the 3D-cursor is where any new spawned object appears at. So wherever that cursor is, any new object added will spawn right on top of it.   

To move the 3D-cursor, we need to **"Shift + Right Click"** at the location we want the 3D-cursor at.

*Initial 3D-cursor location*
![Screenshot](/images/3D_house_tuto1/53.png)

*New 3D-cursor location for Chimney*
![Screenshot](/images/3D_house_tuto1/54.png)

**"Shift + A"** to add new mesh and add a **Cube**. As you would see it spawns right where we put our 3D-cursor.

*Cube spawned right on top of the 3D-cursor*
![Screenshot](/images/3D_house_tuto1/55.png)

Press **"S"** to **Scale** the cube down until you are satisfied with the size. **"Tab"** back into Edit Mode, **"1"** to go to front view, **"Z"** and move to *Wireframe* mode and press **"S"** and **"Z"** to scale the cube on the Z-axis.

*Chimney added*
![Screenshot](/images/3D_house_tuto1/56.png)

## Modeling The Inside Of Our Chimney

**"Tab"** to Edit Mode, choose *Face select* at the top left and choose the upper face of the chimney. Now we press **"I"** for **Inset** and it will create a face within our face so that we can extrude it later on. Once the face has been inseted and validated, press **"E"** to **Extrude** and extrude downwards to form the hole of the chimney.

*Inset added*
![Screenshot](/images/3D_house_tuto1/57.png)

*Extrusion added*
![Screenshot](/images/3D_house_tuto1/58.png)

**Note:** When entering Extrude Mode after Inseting our face, the extrude will be automatically set to move along the Z-axis.

# Adding A Little Foundation To The House

We need to put the 3D-cursor back at the center and for that there is a little handy shortcut which is **"Shift + C"**. Once that's done press **"Sift + A"** to add a new Mesh -->> Cube and scale it down with **"S"** then **"Z"** and choose the thickness you want for the foundation.

*Cube added and enlarged just a bit*
![Screenshot](/images/3D_house_tuto1/59.png)

*Cube shrinked along the Z-axis*
![Screenshot](/images/3D_house_tuto1/60.png)

*Foundation brought down and enlarged for better visuals*
![Screenshot](/images/3D_house_tuto1/61.png)

# Making A Door Frame

Select the house and go to Edit Mode. Go to Vertex Select at the top left and select the loop around the door with **"Alt + Left Click"**.

![Screenshot](/images/3D_house_tuto1/62.png)

Once it's selected like this, duplicate it with **"Shift + D"** and right click right after to cancel its movement. Press **"P"** to make it its own object then select it so that we can start working on it.

*Making the duplicated door it's own object*
![Screenshot](/images/3D_house_tuto1/63.png)

*The duplicated door selected to start working on it in Edit Mode*
![Screenshot](/images/3D_house_tuto1/64.png)

Scale the door frame with **"S"** just a tiny bit, scale it again on the X-axis.

![Screenshot](/images/3D_house_tuto1/65.png)

Now we move it back with **"G"** and **"Y"**

![Screenshot](/images/3D_house_tuto1/66.png)

We extrude with **"E"** then **"Y"** and bring it out just a bit.

![Screenshot](/images/3D_house_tuto1/67.png)

Once this step is done make sure to select everything again with **"A"**. Press **"E"** to extrude and then **"S"** to scale what has been extruded.

![Screenshot](/images/3D_house_tuto1/68.png)

It's not perfect so to make it perfect we repeat **"E"** to extrude and then **"S"** to scale what has been extruded then we press **"Shift + Y"** to scale but not on the Y-axis. Just the X and Z-axis.

![Screenshot](/images/3D_house_tuto1/69.png)

*Result in Object Mode*
![Screenshot](/images/3D_house_tuto1/70.png)

# Changing MatCap

To change MatCap you simply click at the top right, on an arrow key.

![Screenshot](/images/3D_house_tuto1/71.png)

When applying a MatCap you should check whether it's correctly applied or not and to do you simply need to check this:

![Screenshot](/images/3D_house_tuto1/72.png)

All the things in red are the outside mesh and it is supposed to be inside and all the blue is the right side of the mesh. So we can see our door is red whereas it needs to be blue so we need to change that.

To flip it upside down we first of all go back to Edit Mode while the door/frame is selected and press **"Shift + N"** to **Recalculate Normals**

*Door selected*
![Screenshot](/images/3D_house_tuto1/73.png)

*Normals recalculated*
![Screenshot](/images/3D_house_tuto1/74.png)

# Making A Window Frame

Select the house and go to Edit Mode. Go to Vertex Select at the top left and select the loop around the window with **"Alt + Left Click"**.

![Screenshot](/images/3D_house_tuto1/75.png)

Once it's selected like this, duplicate it with **"Shift + D"** and right click right after to cancel its movement. Press **"P"** to make it its own object then select it so that we can start working on it.

*Making the duplicated window it's own object*
![Screenshot](/images/3D_house_tuto1/76.png)

*The duplicated window selected to start working on it in Edit Mode*
![Screenshot](/images/3D_house_tuto1/77.png)

Only select the duplicated window and go to Edit Mode so that it is the only object affected.

* Press **"S"** to scale it so its just a tiny bit larger. 
* Press **"G"** then **"Y"** to move it back just slightly.
* Press **"E"** to extrude then **"Y"** to extrude on the Y-axis. Bring it over just a little bit.

*Result after these steps*
![Screenshot](/images/3D_house_tuto1/78.png)

* **"A"** to select everything.
* **"E"** then **"S"** to scale the extrusion then again press **"Shift + Y"**.

*Result after these steps*
![Screenshot](/images/3D_house_tuto1/79.png)

* **"A"** to select everything then **"Shift + N"** to recalculate normals.

Do the same for the other window.

## Adding A Cross on our windows

* **"Shift + Right Click"** to change the position of the 3D-cursor to where we want it to be.

![Screenshot](/images/3D_house_tuto1/80.png)

* **"Shift + A"** to add a new Mesh -->> Cube.
* Scale it down with **"S"**.
* Scale it on the Z-axis with **"S"** then **"Z"** to form a long bar shape.
* Move it up with **"G"** until it divides the window in half.
* If its too thick for your liking, press **"S"** then **"Shift + Z"** to scale it on both the X and Y-axis but not the Z-axis.

![Screenshot](/images/3D_house_tuto1/81.png)

* The object is already selected so duplicate it with **"Shift + D"**.
* Right click to cancel its movement.
* **"R"** then **"X"** to rotate it on the X-axis.
* Type in **90** and press Enter to rotate it by 90° exactly.

![Screenshot](/images/3D_house_tuto1/82.png)

* Since its a little bit short scale it with **"S"** then **"Y"**.

![Screenshot](/images/3D_house_tuto1/83.png)

### Duplicating The Cross To Put On The Second Window

* Select both the polls with **"Shift + Click"**.
* Press **"7"** to go to top view.
* Hold down **"Z"** to go to Wireframe mode.
* **"Shift + D"** to duplicate the cross and place it on the other window.
* Focus back on the object with **"²"** and you can go back to solid mode.

![Screenshot](/images/3D_house_tuto1/84.png)

![Screenshot](/images/3D_house_tuto1/85.png)

# Adding A Window Pane

* Select the house. Go to Edit Mode.
* Go to Wireframe mode.
* Select the loop around both windows.
* Duplicate them and right click to cancel movement.
* **"P"** to separate them by selection.
* Go back to Object Mode, select the newly duplicated windows and tab into Edit Mode.

![Screenshot](/images/3D_house_tuto1/86.png)

* Go back to Solid Mode.
* To fill the faces of the windows press **"F"** to **Fill Face**.

![Screenshot](/images/3D_house_tuto1/87.png)

Make sure the window cross is not covered by the newly added face.

# Adding A Door

* Select the house. Go to Edit Mode.
* Go to Wireframe mode.
* Select the loop around the door.
* Duplicate it and right click to cancel movement.
* **"P"** to separate it by selection.
* Go back to Object Mode, select the newly duplicated door and tab into Edit Mode.

![Screenshot](/images/3D_house_tuto1/88.png)

* Go back to Solid Mode.
* Fill the face with **"F"**.

![Screenshot](/images/3D_house_tuto1/89.png)

# Adding A Door Handle

* **"Shift + Right Click"** to change the location of the 3D-Cursor and put it where the door handle shall be.
* **"Shift + A"**, Mesh -->> Circle since the circle is the closest thing to a door handle.

![Screenshot](/images/3D_house_tuto1/90.png)

When adding a circle the menu above pops up. We need to change the vertices from **32** to **8** and press enter.

* Scale it down and focus on it to see it better.
* Rotate it sideways with **"R"** then **"X"** and type in **90**.

*Result uptil now*
![Screenshot](/images/3D_house_tuto1/91.png)

* Bring it back slightly with **"G"**.
* Extrude it out.
* Select the loop around the circle like this:

![Screenshot](/images/3D_house_tuto1/92.png)

Now we need to model the handle. For that we go to Wireframe mode and top view to have a better view of our object.

* Scale it up with **"S"**
![Screenshot](/images/3D_house_tuto1/93.png)

* Move it up with **"G"**
![Screenshot](/images/3D_house_tuto1/94.png)

* Extrude it with **"E"**
![Screenshot](/images/3D_house_tuto1/95.png)

* Scale it up a little bit more with **"S"**
![Screenshot](/images/3D_house_tuto1/96.png)

* Extrude it with **"E"**
![Screenshot](/images/3D_house_tuto1/97.png)

* Scale it down with **"S"**
![Screenshot](/images/3D_house_tuto1/98.png)

* Extrude it with **"E"**
![Screenshot](/images/3D_house_tuto1/99.png)

* Scale it down with **"S"**
![Screenshot](/images/3D_house_tuto1/100.png)

Go back to solid mode and fill the face with **"F"**.

Move it around as you wish but once you're done right click and choose **"Shade Smooth"**.
![Screenshot](/images/3D_house_tuto1/101.png)

## Smoothing The Handle With A Modifier

![Screenshot](/images/3D_house_tuto1/102.png)

*Modify the digits as you wish but both of them should be the same*
![Screenshot](/images/3D_house_tuto1/103.png)


![Screenshot](/images/3D_house_tuto1/104.png)

**Note:** You need to apply the modifier to see the result.

*Result*
![Screenshot](/images/3D_house_tuto1/105.png)

# Adding A Ground Plane

* **"Shift + A"**, Mesh -->> Plane.
* Scale it up.
* Bring it down.

*Final House after this first tutorial*
![Screenshot](/images/3D_house_tuto1/106.png)