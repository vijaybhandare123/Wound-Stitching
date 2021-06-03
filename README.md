# Wound-Stitching
This is my first project in Techport ... 

This project is related to providing a stitches to wounds .

At first , the mask is created for the wound in image by using Open CV Library .

When you run the first lines of logic for masking, a window will be opened , where trackbars are given to create a mask .

Trackbars are required as , intensity of redness for images to images is varying , and its get diffucult to finalize same lower and upper values of HSV for all images .

For Red color wound , first we need to move only lower Saturation (s) and then Lower value (v) , and if required , reduce higher value of Hue (H)

If you see the correct mask , then press "esc" button to close the window .

After that , in Logic , Max Contour is found , which correctly encloses the mask .

After thar , ellipse is fitted to that contour and found the angle(direction ) of wound through ellipse details .

Then logic is set to put lines perpandicular to major axis of ellipse and the same lines will intesect to contour .

Found out the intesecting points and then draw a final line .

All this kept in loop , to draw the equidistant lines acoording to shape of image .

Final Result is shown at end .

Result depend on the correctness of mask .
