---
layout: post
title: Geometrical Pattern Using Grasshopper and Paneling Tools
description: How to create a geomatrical pattern using Grasshopper and Paneling Tools
modified: 2016-05-29
tags: [grasshopper rhinoceros]
---
## What is Grasshopper?

Grasshopper is a plug-in for the Rhinoceros 3D modeling software. It has its own interface that generates parametric drawings in rhino. Though Grasshopper it is possible to easily modify a model and create several alternative proposals.

## What is Paneling Tools?

Paneling tools is a Grasshopper’s plug-in. It is a tool to create and manipulate rectangular grids where you can put any form to be repeated regularly through a surface. It can be used both for 2D and 3D models.

## Box Pattern

The pattern modeled by me using Grasshopper will be used as a decorative drawing for a simple box. It will have three different pieces that will be cut and engraved with a laser cutter.

<figure class="half">
	<img src="/images/box.jpg" alt="">
	<img src="/images/box2.jpg" alt="">
	
<figure class="half">
	<img src="/images/box3.jpg" alt="">
	<img src="/images/box4.jpg" alt="">
	

For the pattern, it was used the command rectangle to create a boundary for the geometry to be created. Then, I made a diagonal line from the center of the square until one of its corners. To do that I used the command Area to find the center of the square and Divide Curve with a number slider 8 to find the corner and mid points. Then I drew a line. After that, I found the midpoint of this line using divide curve again with a number slide 2, drew a perpendicular line and used the command evaluate length to create a point that can be moved through this line. Then I made an arc using this point, the center point and the corner point. I mirrored the arc, joined the two arcs and used the command polar array to get the flower shape.

<figure>
<img src="/images/unit.jpg" alt="">
</Figure>

For the grid I used the commands Planar Grid, Cellulate and Morph 2D from Panneling Tools and plugged my geometry to it and got the desired pattern.
Modifying the number plugged to the evaluate length and the polar array commands changes the final shape of the pattern.

<figure class="half">
	<img src="/images/Pattern1.jpg" alt="">
	<img src="/images/pattern2.jpg" alt="">
	
<figure class="half">
	<img src="/images/pattern3.jpg" alt="">
	<img src="/images/pattern4.jpg" alt="">

<figure class="half">
	<img src="/images/pattern5.jpg" alt="">
	<img src="/images/pattern6.jpg" alt="">


Below is an image that shows how it looks like on Grasshopper

<figure>
<img src="/images/Grasshopper1.png" alt="">
</Figure>
