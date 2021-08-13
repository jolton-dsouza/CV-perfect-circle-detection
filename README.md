## Perfect circle frame detection from noisy video
Given a video, find the frame which has perfect circle


### Dependencies
-Python3
-OpenCV – 3.4.15
-numpy - 1.12.0
-skimage 


### Algotithm
1. Use Hough Transform to detect a circle of certain radius
2. Dilate the Hough Transform circle
3. Use Active Contours/Snakes algorithm to fit the shape around the inner circle
4. Using the contour and OpenCV moments, find the centroid
5. Using all points on the circumference of the shape, find Roundness Ratio(=1 for perfect circle)


