# AR in Real-Time-Frame
Augmented reality based application using Python, numpy and OpenCV

> Make Sure You Run these Commands in Terminal (or have it installed already)
 ```
 pip install opencv-python
 pip install numpy
 pip install easydict
 pip install objloader
 ```
> *I have worked using python 3.7, different versions can demand other libraries and a slightly different code*

## Usage

* Place the image of the surface to be tracked inside the `reference` folder.
* In the code, replace `'model.jpg'` with the name of the image you just copied inside the `reference` folder.
* Replace `'fox.obj'` with the name of the model you want to render. To change the size of the rendered model change the scale parameter (number `3`) by a suitable number. This might require some trial and error.
* Open jupyter notebook inside the project folder and run `AugmenetedReality_in_RealTime.ipynb.
* Press `esc` to quit the output window


### Command line arguments

* `--rectangle`, `-r`: Draws the projection of the reference surface on the video frame as a blue rectangle.
* `--matches`, `-m`: Draws matches between reference surface and video frame.


# Scope 
* to project in a screen a 3D model of a figure whose position and orientation matches the position and orientation of some predefined flat surface.
* to do it in real time, so that if the surface changes its position or orientation the projected model does so accordingly.

### This can be done integrating the task:
1.  Recognize the reference flat surface.
2.  Estimate the homography.
3.  Derive from the homography the transformation from the reference surface coordinate system to the target image coordinate system.
4.  Project our 3D model in the image (pixel space) and draw it.

For each step there could be many amazing algorithms implementing various methods of
* feature detection,description and matching
* estimation of homography and projection

***feel free to choose any !!!***
