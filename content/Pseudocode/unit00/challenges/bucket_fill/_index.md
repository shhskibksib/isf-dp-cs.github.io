---
title: Bucket Fill
weight: 10
# draft: true

---


# Bucket Fill Challenges


## Setup

To keep your workspace clean, start by creating a new java project in Eclipse called "Bucket Fill". You will put the methods you write in this project.

## Square
This one should be quick and easy. You are given the coordinates of the 4 corners of the square.You are also given the coordinates of one pixel. Tell the user whether the pixel is *inside* the square or not.


- [ ] ***Write the method `insideSquare()`***
- [ ] ***Parameters: `xPt1`, `yPt1`, `xPt2`, `yPt2`, `xPt3`, `yPt3`, `xPt4`, `yPt4`, `xPixel`, `yPixel`***
- [ ] ***Return: `True` or `False`*** 


## Circle
It only takes 3 points to define a circle. Your task will be to determine if the pixel is *inside* the circle or not.


- [ ] ***Write the method `insideCircle()`***
- [ ] ***Parameters: `xPt1`, `yPt1`, `xPt2`, `yPt2`, `xPt3`, `yPt3`, `xPixel`, `yPixel`***
- [ ] ***Return: `True` or `False`***  

## Convex Polygon
This time all you get is a list of vertices. You don't know how many there will be. All you know is that the polygon is convex (luckily). Your task will be to determine if the pixel is *inside* the polygon or not.

- [ ] ***Write the method `insideConvexPolygon()`***
- [ ] ***Parameters: `arrayOfPoints` , `xPixel`, `yPixel`***
- [ ] ***Return: `True` or `False`***  

## Any Polygon
Oh no! Now you don't know if the polygon is convex or not. Your a list of vertices. You don't know how many there will be. All you know is that the polygon is convex (luckily). Your task will be to determine if the pixel is *inside* the polygon or not.

- [ ] ***Write the method `insideAnyPolygon()`***
- [ ] ***Parameters: `arrayOfPoints` , `xPixel`, `yPixel`***
- [ ] ***Return: `True` or `False`***  