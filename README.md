# Udacity_Autonomous_Driving_NonDegreeProgram_P1

#  Finding Lane Lines on the Road

## Summary of 5 main steps of pipline

###  *1*, apply grayscale transform.  *2*, apply a Canny Edge Detector to indentify edges in images.  *3*, I reduce the noises of images by using GaussianBlur.  Any point beyond the max threshold will be included in the resulting image while edges below min threshold are discarded.  *4*, determine a region of interest and discard any lines outside of this polygon. One crucial assumption in this step is that the camera remains in the same place across all these image, and lanes are flat.  *5*, apply ** Hough Transform** to find lines by identifying all points that lie on them. 

## Shortcomings of pipline

### *1*, straight lines do not work when there are curves on the road

### *2*, hough transform is tricky to get right with its parameters. Not quite sure got the best settings.

## Possible improvements of  pipeline

### *1*, pay more attentions to the pixels next to edges and include the points next to edges but beyond max threshold. This may be helpful for getting a more continous straight line.
### *2*, combining the draw_lines() function with the weighted_img() can  make the lines semi-transparent, which is way  worthing of trying.

# Codes Result Display
## Markdown currently does not support for enbeding video file in a readme so put this URL linking to a youtube video displaying the result.
[![Video Display for Autonomous Driving Finding Lanes Works](https://user-images.githubusercontent.com/40772712/56013701-10645d80-5cc0-11e9-8c0a-e188bf3cd068.PNG">)](https://www.youtube.com/watch?v=5nM1JaeyceE&feature=youtu.be)
