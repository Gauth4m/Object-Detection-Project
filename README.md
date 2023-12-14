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



# Object detection using TensorFlow Model 

System Requirements for training the model: Computer with Gpu (Nvidea suggested).

Please combine this installation guide with "TFLite2_Object_Detction_Model.ipynb" file.

Step 1. Download and Install Anaconda

##
https://www.anaconda.com/products/distribution

Step 2. Set Up Virtual Environment and Directory

Now we need to create a new folder directly in :c drive with the name "tflite1".
Copy and paste the zip ipynb downloaded file to that folder. 

Now open Anaconda Prompt terminal and move into it by following command 

##
mkdir C:\tflite1
cd C:\tflite1

Next, create a Python 3.9 virtual environment by issuing:

##
conda create --name tflite1-env python=3.9

Enter "y" when it asks if you want to proceed. Activate the environment and install the required packages by issuing the commands below. We'll install TensorFlow, OpenCV, and a downgraded version of protobuf. TensorFlow is a pretty big download (about 450MB), so it will take a while.

##
conda activate tflite1-env
pip install tensorflow opencv-python protobuf==3.20.*

Download the detection scripts from this repository by issuing:

curl https://raw.githubusercontent.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi/master/TFLite_detection_image.py --output TFLite_detection_image.py
curl https://raw.githubusercontent.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi/master/TFLite_detection_video.py --output TFLite_detection_video.py
curl https://raw.githubusercontent.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi/master/TFLite_detection_webcam.py --output TFLite_detection_webcam.py
curl https://raw.githubusercontent.com/EdjeElectronics/TensorFlow-Lite-Object-Detection-on-Android-and-Raspberry-Pi/master/TFLite_detection_stream.py --output TFLite_detection_stream.py


Step 3. Move TFLite Model into Directory


##
tar -xf custom_model_lite.zip


Step 4. Run TensorFlow Lite Model!


##
python TFLite_detection_webcam.py --modeldir=custom_model_lite


This command will open the web cam to detect the coins. 


How to train and download ipynb file using tensorflow module in google colab 
https://www.loom.com/share/16f4bd954f384b549074d65e0307a9fd?sid=31eb1ba8-9b94-4ad2-939b-a709c102fe2e

How to open downloaded ipynb file in a computer. 
https://www.loom.com/share/b2db203132e8420b92b35c613d735a14


