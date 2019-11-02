# AR in Real-Time-Frame
Augmented reality based application using Python, numpy and OpenCV

> Make Sure You Run these Commands in Terminal (or have it installed already)
> * pip install opencv-python


## Usage

* Place the image of the surface to be tracked inside the `reference` folder.
* In the code, replace `'model.jpg'` with the name of the image you just copied inside the `reference` folder.
* Replace `'fox.obj'` with the name of the model you want to render. To change the size of the rendered model change the scale parameter (number `3`) by a suitable number. This might require some trial and error.
* Open jupyter notebook inside the project folder and run `AugmenetedReality_in_RealTime.ipynb.
* Press `esc` to quit the output window


### Command line arguments

* `--rectangle`, `-r`: Draws the projection of the reference surface on the video frame as a blue rectangle.
* `--matches`, `-m`: Draws matches between reference surface and video frame.



