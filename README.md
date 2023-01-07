# Image_Tampering_Detection

This script appears to be using the structural similarity index (SSIM) to compare an original image of a PAN card to a user-provided image, 
in order to determine whether the user-provided image is an original or tampered version of the PAN card.

The script begins by loading the original and user-provided images and converting them to grayscale. 
It then calculates the SSIM between the two images, which is a measure of the structural similarity between the two images. 
The script also generates a difference image, which shows the differences between the two images.

Next, the script applies an adaptive threshold to the difference image and uses the cv2.findContours() function to identify the contours in the image. 
The script then loops over the contours and draws them on the images to highlight the areas of difference between the two images.

Finally, the script displays the original, tampered, and difference images, along with the SSIM score, 
in order to allow the user to visually inspect the results of the comparison. If the SSIM score is low, 
it may indicate that the user-provided image is a tampered version of the original PAN card.
