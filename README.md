# GrainPheno
An image analysis based tool for measuring grian size

GrainPheno is an image analysis-based tool for counting and measuring grain size. GrainPheno provides a standalone version for running on personal computers of windows systems, and a WeChat based applet for analyzing gain images on smartphones. Thus, grain images acquired from scanners and mobile imaging devices are supported to be analyzed by GrainPheno. 

1 Installation

(1) Install on personal computer with Windows system
Download the soft and test files from the GitHub website (https://github.com/xiexr/GrainPheno). Decompress the soft file to the local disk, for example D:\ or others, and the path should not contain special characters. Enter the directory of GrainPheno, and double click the “GrainPheno.exe” to run the program. 
GrainPheno provides test files in the GitHub. According to the instruction to input the test files and run the program for testing whether the installation is successful.
(2) WeChat applet
Search the applet in WeChat using the ID name: GrainPheno

2 Quick start
 
2.1 Input grain images
Click the “File>Open” in the menu, or click the “File” button on the toolbar to input the images. Select grain images in the file input dialog. The file name and corresponding path should not contain special characters. 
 
2.2 Necessary setting for running
(1) Background color
GrainPheno provides two background colors, including black and white. For grains with light color, black background is suggested; otherwise, white background is suggested. 
 
(2) Model
The parameters of “Model”, which are detailed explained below, have impact on the accuracy of measurement. Currently, GrainPheno provides four models, including Default, Rice, Maize, and Soybean, for users. Users can open the “Configure setting” dialog from the menu, and modify, add or remove model.
 
(3) Ruler length（default value is 100mm）
Users need input the ruler length for GrainPheno to calculate exact size of grains. The length should be larger than the length of grains, such as 50 mm or 100 mm. To estimating the horizontal balance of images captured by mobile imaging devices, such as cameras and mobile phones, two rulers are suggested to place on the background.
 
2.3 Image crop (optional)
GrainPheno incorporates the useful function for users to crop images. Click the “Crop” button on the toolbar to open the crop dialog, and drag the mouse to select the image region for analyzing. By choosing “Apply the crop region to all figures”, users can apply the region to all input images. 
 
2.4 Run
Click the “Run” button to run the program. During the running procedure, related processing information and running results, including the result directory info, are displayed in the “Info” region.
 
2.5 Zoom (optional)
By dragging the “Zoom” button, users can zoom the image to view the detailed region of image.
 

2.6 Result files
The resulting files are automatically saved in the same file of input images. Users can also see the result directory information from the “Info” region, which is indicated with “All results have been saved to directory: (directory name)”. 
The results files include:
(1) The measured size of normally grains. The file name is: <image name>_ normal.result.xlsx.
(2) The measured size of abnormally grains. The file name is: <image name>_ abnormal.result.xlsx.
(3) The result image (file name is: <image name>_.result.jpg or .png file), in which normally recognized grains are indicated with red rectangles, abnormally recognized grains are indicated with green rectangles. The rule(s) are indicated with blue rectangle(s), and the numbers in white color indicates the grain ID.
 

3 Detailed descriptions
3.1 How to obtain a high-quality grain image?
(1) Please use a black background for grains with light color; otherwise, please use a white background.
(2) The length of ruler(s) should be longer than that of grains, which 50 mm or 100 mm are suggested. 
(3) Please place the grains unevenly on the background as much as possible.
(4) Please keep the horizontal level between the grains and the mobile imaging devices, such as smartphones or cameras. 
3.2 How to crop images?
GrainPheno provides the crop function for users to process grains images. After clicking the “Crop” button on the toolbar, the dialog of image crop pops up. Please select the desired region by dragging the mouse, and the crop region will be applied to all input figures if uses choose “Apply the crop region to all figures”.
 
3.3 Set the parameters for models
Click the “Seeting> Set the parameters of models” in the menu to open the dialog for modifying, adding or removing models. 
 
Explanation for the parameters in the model dialog:
Aperture size of median filter: it has influence on the effect for removing scratches on the background. A larger aperture size is suggested for images with obvious scratches. The value should be in odd number.
Block size of binarization: usually no adjustment is required.
Threshold of binarization: it affects the accuracy of grain contour.
Kernel size of morphology open: it used for removing attachments on the grains, such as spike or awn. Try to set an appropriate value that can remove the attachments, while not affect the accuracy.
Minimum seed area: it used for removing scratches on the background. Increase the value to remove scratches, or decrease it to make the grains detectable.
Minimum defect size: it has influence on the segmentation of adhesive grains. Please try to decrease the value if adhesion is failed to be correctly separated; otherwise, try to increase the value if over-segmentation happed. 

Contact:
Xianrong Xie: xiexianrong@scau.edu.cn
Haoran Zhan: 1138412533@qq.com 
