Download link: https://pan.baidu.com/s/1oarB7VfPkr_UHPPHfennww?pwd=gdsb
Please read this documentation before using the SAXSNN.exe program

1. Prepare the dataset
Create a new folder and place the grayscale images (require .tif format!!!) of the SAXS data that need to be calculated into it. Create a data.dat file in the same directory, label the SAXS images in order and name them with numbers (1-n.tif). Enter the names into the. dat file as follows:
1
2
3
...
n

2. Run the SAXSNN.exe
Path choice: 
1.Select the file path where the dataset is located
2.Choose the output path of the result file, preferably not the same as the dataset folder
3.The prefix for naming the main results

3. Model parameter：
Note that the input image pixel resolution of this program needs to be greater than 256 * 256, and the default output size is 256 * 256。
Model iteration epochs: The larger the number of iterations, the longer the calculation time. The default iteration times are 5000 epochs.
Learning rate: The larger the value, the fewer iterations required, but the stability of the results decreases. The default value is 0.00005.
Center occlusion size: This parameter is mainly used for data related to overflow occlusion of the center through light. It can be used to occlude high-intensity signals in the center. If not needed, please enter 0.
Be careful !!!!!! 
Due to the long processing time required for large batches of data, it is recommended to firstly use a single image to test the rationality of parameters and calculation time, and then perform batch processing on the entire dataset.

4. Start extracting data:
Click the button. 
If the IDs of all image data are displayed, it proves that the data has been successfully imported. 
If there is an error, please check the 1.step of this document.

Start running, please be patient and wait for the pop-up message 'Calculation completed' to appear. The calculation process is viewed in cmd.
