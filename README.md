Please combine this installation guide with "YOLOv5_Object_Detection.ipynb" file.

# Object-Detection-Project via YOLOv5 model
1. There is a link on top of the codes that brings you to Google Colab Notebook codes
   * You need to have a Google Account
   * On the setting, on top right of the Google Colab page, you can give permission to connect to GitHub and Google Drive

2. Mount the codes to your Google Drive in order to run the codes in your Drive
   * Give permission if it asks permission to be connected to your Google-Drive
   * Use your own Google-Drive path in the second code line of this cell

3. Install and upgrade Python, pip, Tensorflow, Tensorboard, Torch and import Torch.
   * Prompts that start with "!" are installing the pakages on your computer similar to Commands on Windows and Terminal on Mac.
   * Prompts that start with "%cd" will be installed in that specific shell as a virtual environment

4. Clone YOLOv5 on your Google-Drive
   * It will be cloned on your G-Drive not your local machine
  
6. Install YOLOv5 compatibe package versions 
   * Run the file "reqirement.txt" in the cloned YOLOv5, to install all required package versions.
   * Required packages will be installed in virtual environment at your Google Drive/yolov5.
   
8. Run Object Detection model
   * Create a folder in your Drive/ as source image folder and uploade your images in that folder to be detected
   * Use your source image path in the code
  
9. Show Result
   * Enter the name and path of the detected image which is visible in the last line of previous code after running.
   * Detected objects will be saved each time in a new folder, so the folder path needs to be updated for each run. 
   
Link to video explanation: 
https://www.loom.com/share/d8c3353ad02642e58dd7dfd27a070de2?sid=2243aaae-1397-41ae-9d84-f52f2adb03e8
