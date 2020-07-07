# Self-driving-Car-Basic-Lane-Detection
Lane detection algorithm with OpenCV library of Python with the application to the images and videos

![laneplt](https://user-images.githubusercontent.com/57037068/86800187-d11fea80-c083-11ea-86cb-93dc70eed1a9.png)

After the Canny Edge Detection algorithms is applied to the frames (image) which is previously converted to grayscale (for lowering down the color channels, and lowering the computational power needed), Gaussian blur (5,5) is made on it to remove some noise that can mislead edge detection algorithm. By the way Canny already applies blur to frames as well.
Cropping Region of interest from the frame and masking them eventually.
For defining the lines - Hough Transform and finding intersections in hough space applied
bin - intersections - highest value for intersection - threshold - min val of intersection to decide it as line

After averaging out the lines in the frame according to coordinates, capture is made and all def are applied in the end.

![obc](https://user-images.githubusercontent.com/57037068/86802102-b77fa280-c085-11ea-8853-0756f3278d8f.gif)


