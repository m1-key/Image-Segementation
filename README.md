# Image-Segementation
* This whole program is made to extract the dominant colors of the image and then to recreate the image with those dominant colors.
* K Means Clustering is used here to perform this task.
---
### What is K Means Clustering ?
* This algorithm basically follow 4 steps.
1.  It first randomly intialize centres.
2.  It computes the distance of each point from each center and associates the point to that center from which its Eucledian distance is minimum. (```Euclidean Distance between two points ((x,y),(a,b)) is given as = √(x - a)² + (y - b)²```)
3.  After associating all points with the centers , the value of center is changed. New value of center is the mean value of all the points associated with it. After changing all the centers , the points associated with it are removed.
4.  Step 2 is again performed and then 3 until the optimum state is reached. 
* Each center now associated with some points , now this group of points together is called cluster.
---
* Image segmentation involves few steps mentioned below.
* ``` Reading the image --> converting it into 2D array --> Applying K Means --> Extracting the dominant colors --> Assigning these colors to new image --> Reshaping it into original size. ``` 
---
## Example
``` Let say we have an image in which blue color is dominant , each point in the image is characterized by the pixel and since blue color is dominant , so all the blue color point will have same pixel value. When K means clustering is applied , it groups all those blue color points into a cluster as these points are similar. Similary if an image has more than one dominant color then this algorithm group all the similar pixel points together into a cluster. In this way this algorith helps to find dominant colors of an image. ```

### Note:
IPYNB file contains the example with code.  So go through that to get better intutuion about this algorithm.
