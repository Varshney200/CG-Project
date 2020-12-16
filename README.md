# Computer Graphics - Project (CSE-1, 5th Sem)

## Team Details: 
- 00101012018: Aamiya Garg 
- 01301012018: Archita Varshney
- 01701012018: Sakshi Jain
- 02801012018: Apoorva Gupta
- 02901012018: Vanshika Uniyal

## About the Project:
In this project, we have made a web application wherein we have used a cube to depict rotation about x, y, z-axis, and composite rotations about xy, yz, zx, and xyz axis. We have used orthographic projection to represent a three-dimensional object in two dimensions. We have designed a responsive website using HTML to create the basic layout and JavaScript to depict animations. 

## Working of the Project:

Function Rotate( ): To provide a visual realism of the 3D object after Rotation in 3D view we apply the following transformation.

We consider two rotations
 - about Y-axis by an angle, ɸ
 - about X-axis by angle Ɵ
and then the projection on the Z = 0 plane.

Function cubeAnimateRotate(): This function creates a new transformation matrix for the calculated frame angle(frame angle = rotation speed * time for 1 frame). 
The transformation matrix is calculated as shown in the image. Then this matrix is multiplied by the matrix of coordinates of the cube vertices. This gives us the coordinates of the cube after rotation about the specific axis.
-	cubeAnimateRotateX() gives the coordinates for the cube after rotation about the X - axis.
-	cubeAnimateRotateY() gives the coordinates for the cube after rotation about the Y - axis.
-	cubeAnimateRotateZ() gives the coordinates for the cube after rotation about the Z - axis.
-	Then we show the cube with the transformed vertices using the function drawCube() and finally, we call the cubeAnimateRotate() function again  till the stop button is pressed

Function CubeReset( ): This function will reset the rotation angles and the cube to its position with no transformation applied.
