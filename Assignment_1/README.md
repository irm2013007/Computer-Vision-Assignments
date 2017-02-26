# Computer-Vision-Assignments


##Find length of pen using Camera Caliberation techniques


###Idea Used

We are assuming picture to be taken from camera with some reference matrix in the scene.
That matrix is a square in our case. So we are fixing four reference point(corners of square in real world) namely p1, p2, p3 and p4 respectively.
Then we created a dummy image with some dummy square, with end points lets say q1, q2,q3 and q4 respectively.
Now task was to find a matrix, which is called as HOMOGRAPHY MATRIX, which finds the relation bwtween these points i.e, it helps in converting the real world coordinate system into camera world corrdinate system and vice versa.
Say this matrix is H.

    p1*H = q1
    p2*H = q2
    p3*H = q3
    p4*H = q4
    
    
 Now we know actual length of square in real world i.e,  distance between p1 and p2, say L1 and similarly in camera world say L2.
 
Length of pen in real world = length of pen in camera world * L1/L2;


```

## Prerequisites
```
 - ipython notebook with Python 2.7 and OpenCV 3.0
```

## Description of Code 
```
function saveImage() is used for taking new sample images and saving it in input folder.

function savePoints() will ask user to select points in saved image which are end points of square and end point of pen and store the homography imformation in PerspectiveTransformation folder.

finally block [26] performs the task mentioned above, i.e, converting image into top view and then finding pen lenth in camera view and finally converting that lenght in real world coordinates.


```
## References:
[Technique used] (http://math.stackexchange.com/questions/494238/how-to-compute-homography-matrix-h-from-corresponding-points-2d-2d-planar-homog).







