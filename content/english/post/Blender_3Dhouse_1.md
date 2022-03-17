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
- “Shift + A” to open **Add Menu** and choose Mesh --->> Cube.

![Screenshot](/images/3D_house_tuto1/1.png)

# Object Mode Vs Edit Mode

To switch between Object and Edit mode simply press “Tab”.

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


**Note:** To select multiple vertices, edges or faces, “Shift + Click” to begin selecting multiples.

# Cutting Cube in Half

To cut the cube in half we first go to the top view by pressing "1" and add a **Loop Cut** by pressing "CTRL + R".
Once that's done you choose the orientation of the cut. Either horizontally or vertically.

- *Vertically*

![Screenshot](/images/3D_house_tuto1/7.png)

- *Horizontally*

![Screenshot](/images/3D_house_tuto1/8.png)

Select the face to be deleted and press "X" to delete then choose "Vertices" to delete half of the cube.

- *Before*

![Screenshot](/images/3D_house_tuto1/9.png)

- *After*

![Screenshot](/images/3D_house_tuto1/10.png)

## Mirroring The Cube

Go back to Object Mode by pressing "Tab" and choose **Modifier Properties** on the right:

![Screenshot](/images/3D_house_tuto1/11.png)

Choose the **Mirror** modifier on the dropdown menu:

![Screenshot](/images/3D_house_tuto1/12.png)

When this is done, you can select all objects on the scene with "A" and press "G" to move it:

![Screenshot](/images/3D_house_tuto1/13.png)

We can clearly see the mirrored side is not attached to the orginal one and to change this we need to check the **Clipping** property in the **Mirror modifier** properties:

- *Off*

![Screenshot](/images/3D_house_tuto1/15.png)
![Screenshot](/images/3D_house_tuto1/13.png)

- *On*

![Screenshot](/images/3D_house_tuto1/16.png)
![Screenshot](/images/3D_house_tuto1/14.png)