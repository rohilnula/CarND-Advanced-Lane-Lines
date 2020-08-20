## Advanced Lane Finding

In this project, a software pipeline was built to identify the lane boundaries in a video. Included in the repository is a detailed document explaining the steps followed in the project "Project2_Writeup.pdf".  

The Project
---

The steps involved in the pipeline are as follows:

* Compute the camera calibration matrix and distortion coefficients using a set of chessboard images.
* Apply a distortion correction to raw images.
* Use color transforms, gradients, etc., to create a thresholded binary image.
* Apply a perspective transform to rectify binary image ("birds-eye view").
* Detect lane pixels and fit to find the lane boundary.
* Determine the curvature of the lane and vehicle position with respect to center.
* Warp the detected lane boundaries back onto the original image.
* Output visual display of the lane boundaries and numerical estimation of lane curvature and vehicle position.

The images for camera calibration are stored in the folder called `camera_cal`.  The images in `test_images` are for testing your pipeline on single frames.  If you want to extract more test images from the videos, you can simply use an image writing method like `cv2.imwrite()`, i.e., you can read the video in frame by frame as usual, and for frames you want to save for later you can write to an image file.  

The resultant images generated by the pipeline are stored in `output_images`. The video called `project_video.mp4` was fed to the pipeline and its output is placed in the folder `output_vedios`.  

