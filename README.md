# Polaroid-Photo-Video-Styling-in-Python
Desktop based application for styling images and videos developed in Python using OpenCV and Tkinter mainly . It involves using image 
processing techniques to styling images and videos . So basically , the project consists of two inter-linked parts . Many image processing 
software's are working on animating images and videos. Their available features include cartoonizing images using filters, brushes, 
pencil strokes, and allow users to thicken object edges, blur objects and increase/decrease background cartoon effects. 

## Motivation 
Our project is aimed at giving the videos a pixel art style instead of an animated effect. Also, many
available software's like AKVIS, Adobe After Effects, FilmoraPro and Video Cartoonizer are expensive
and are not portable to multiple OS platforms.
1. Image Styling
2. Video Styling

![image](https://github.com/MuhammadSaqib001/Polaroid-Photo-Video-Styling-in-Python/blob/main/polaroid.png)  

### 1. Image Styling :-
For a photo , we have 5 to 6 pixel art or styling options named as pixelate , swirly ,
cartoonized , pop-art and retro styling . OpenCV was majorly used to give a cartoon effect to the
images by interpolating, creating edge masks, reducing the color palette, smoothing and finally
combining the edge masks with the colored image .

### 2. Video Styling :-
1. Background/ Foreground Identification :-
Given a video as a user input, the program prompts the user to draw foreground using green and
background using red paint brush. This is done to assist the program in roughly classifying which
pixels the user wants to keep as background or the foreground. It then runs k means clustering and
stores the foreground and background centers in a csv file. It uses those centers to blackout the
background hence separating it from the foreground all while the video is playing.

2. Applying Styling Effects :-
This part is the most computationally heavy one. It takes user input at first. It then extracts all the
frames from the video and appends it to an array. The array is then passed to any styling effect
which applies the effect to every single frame. And finally, the last part of the code stitches it back to
make the final styled output video.

## References :-
1. https://towardsdatascience.com/turn-photos-into-cartoons-using-python-bb1a9f578a7e
2. https://data-flair.training/blogs/cartoonify-image-opencv-python/
3. https://stackoverflow.com/questions/55508615/how-to-pixelate-image-using-opencv-in-pytho
4. https://stackoverflow.com/questions/47143332/how-to-pixelate-a-square-image-to-256-big-pixels-with-python
5. https://www.codegrepper.com/code-examples/python/frameworks/-file-path-python/how+to+play+video+in+opencv+python
6. https://www.proquest.com/docview/1441936888/fulltextPDF/6699167900684A54PQ/1?accountid=135034
7. https://pysource.com/2018/10/11/how-to-create-a-cartoon-effect-opencv-with-python/
8. https://dl.acm.org/doi/pdf/10.1145/987657.987676
9. https://dl.acm.org/doi/pdf/10.1145/2071423.2071500
