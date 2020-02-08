# DetectingTomatoPlantDisease
I created a python to detect plant diseases using keras and machine learning methods. The data I used to train the found can be found on Kaggle here: https://www.kaggle.com/charuchaudhry/plantvillage-tomato-leaf-dataset#0045ba29-ed1b-43b4-afde-719cc7adefdb___GCREC_Bact.Sp%206254.JPG

#  Steps:
To make the code work on your machine, follow the steps listed:

1. Download python from python.org, and install all the required libraries via pip.
This step is pretty self explanatory. To install python, go to python.org and navigate to the appropriate download for your OS and hardware. I used python 3.8 at the time of this project, but any python 3 version should work. When installing python, make sure the add pip to line option checked. Using pip, install all dependenices, including jupyter notebook as it will be the easiest way to run my code.

2. Download Kaggle Data Set
Click on the attached link and press the download button. The file should come in .zip format. Make sure to unzip the contents to a new folder

3. Slight Code Change
Depending on the OS, there is a slight change in the code that needs to be made. If on windows, the code should work as is, but if on MacOs, there is one technicality in the script that must be changed. On line 21 of the first block, locate the statement: 
label = str(folder_dir).split("\\")[-1]. If you are on MacOs, change the double backslash to a single forward slash.

4. Extra Note
When I initially trained this model, I recieved a valdiation accuracy of about 30% with a training accuracy of about 97%. This strongly suggests that there is overfitting in the data. This means further techniques have to be implemented to reduce the overfitting, such as reducing the number of epochs and creating artificial data based off of the existing data using image manipulation.
