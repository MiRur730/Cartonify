   Name-MITALI RAJPUT 
   ROLL NO-102118067
   BRANCH-CSBS3


TITLE- CARTOONIFYING AN IMAGE

THIS WHOLE ELC PROJECT IS BEING DONE BY ME IN VSCODE USING PYTHON LANGUAGE .
IT INVOLVES INSTALLATION OF VARIOUS LIBRARIES .
Tkinter , easygui, matplotlib , os ,opencv.
MOST IMPORTANT OF ALL WAS OPENCV (cv2).

IN THIS PROJECT WE WILL MTAKE A NORMAL IMAGE AND CONVERT IT TO A CARTOONIFIED VERSION OF IMAGE 


VARIOUS STEPS INVOLVED ARE

STEP 1
CONVERTING NORMAL IMAGE TO A SKETCH VERSION WHERE THE EDGES OF THE IMAGE HAS PENCIL SKETCH FORMAT

STEP 2
 CREATING A  NEW IMAGE WITH COLOURS BEING QUANTISED AND REDUCED
  TO MAKE IT LOOK LIKE PAINTING .

THEN BOTH THE SKETCH AND PAINTING IMAGE IS MERGED AND LAYERED TOGETHER TO GIVE IT A CARTOONIFIED LOOK.

In the beginning of the project tkinter object top is being created which basically provides a graphical user interface a small window with option of uploading image to be cartoonified
I have also added an option of saving image with name as cartoonified image
Easygui helps to open the box to choose the file and help us to store path as string in image_path variable created and sent this path to cartoonify function


cartoonify will take this path of image in short image being selcted by us
and read it using imread by cv2 library help and storing it in form of numbers (matrix) then converting to RGB format.
convert it into gray scale image ,in simple words image will have only grey color similar to saying colourless.
I am resizng image every single time ,I am making changes into it.
Though i have commented plt.show() - it helps in showing image after each and evry step.

Next Step-Bluring image using medianBlur.
Then i am retrieving the edges of the image and highlighting them. This is attained by the adaptive thresholding technique. The threshold value is the mean of the neighborhood pixel values area minus the constant C. C is a constant that is subtracted from the mean or weighted sum of the neighborhood pixels. Thresh_binary is the type of threshold applied, and the remaining parameters determine the block size.

We use bilateralFilter which removes the noise. It can be taken as smoothening of an image to an extent.
Combining the two specialties will be done by  using MASKING.


Then created a list by name images stored and plotted all the steps images
saved using imagepath from where image was taken and uploaded from with title cartoonified.


THANK YOU ,
Respected ELC MEMBERS for giving me this great opportunity to explore new field of Image Processing.

