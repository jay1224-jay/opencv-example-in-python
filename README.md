## example

Before running this program, make sure you have install ```opencv-contrib-python``` in your computer.

If not, run this command to install it: 

``` 
pip install opencv-contrib-python
```

After that, you have to set the video source which opencv will use:

in Line 46

```python
# Read video
video_path = "test.mkv"
# video = cv2.VideoCapture(video_path)
video = cv2.VideoCapture(0)  # use camera as video source
```

If you would like to use your camera as your video source, you don't have to do any change since the default setting is to use the camera.

If you want to use your video file(such as .mp4, .mkv, ...), you must do this change: 

```python
video = cv2.VideoCapture(video_path)
# video = cv2.VideoCapture(0)  # use camera as video source
```


Now, you can execute the program:

```
python3 main.py
```

It will pop up a window where you can select a region that opencv will keep tracking.

Hit enter to continue.

Bang~. You will see another window displaying the tracking progress with a bouding box (the blue one) and a direction arrow (the green one).

Reference: 

https://learnopencv.com/object-tracking-using-opencv-cpp-python/
