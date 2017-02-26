# Computer-Vision-Assignments


## Assignment1: Camera Calibration



## Idea Used

We are assuming picture to be taken from camera with some reference matrix in the scene.
That matrix is a square in our case. So we are fixing four reference point(corners of square in real world) namely p1, p2, p3 and p4 respectively.
Then we created a dummy image with some dummy square, with end points lets say q1, q2,q3 and q4 respectively.
Now task was to find a matrix, which is called as HOMOGRAPHY MATRIX, which finds the relation bwtween these points i.e, it helps in converting the real world coordinate system into camera world corrdinate system and vice versa.
Say this matrix is H.
So ,
    p1*H = q1
    p2*H = q2
    p3*H = q3
    p4*H = q4
    
    
 Now we know actual length of square in real world i.e,  distance between p1 and p2, say L1 and similarly in camera world say L2.
 
 so length of pen in real world = length of pen in camera world * L1/L2;
```

## Prerequisites
```

- Opencv 3.0.0
- Anaconda with python 2.7
```


## Input 
```
Folder named as "input" contains different input images of pen.
```




## How to use run code 
```
- Open jupyter notebook
- Then run the file named as "Camera_Calibration.ipynb".
```
## References:
[Technique used] (http://math.stackexchange.com/questions/494238/how-to-compute-homography-matrix-h-from-corresponding-points-2d-2d-planar-homog).







