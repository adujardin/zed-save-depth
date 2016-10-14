# zed-save-depth

**This sample is designed to work with the ZED stereo camera only and requires the ZED SDK. For more information: https://www.stereolabs.com**

This sample allows you to save depth information provided by the ZED Camera or by an SVO file, in different formats (PNG 16-Bit, PFM, PGM, XYZ, PCD, PLY, VTK).

This sample requires OpenCV.

## Build the program

Open a terminal and execute the following command:

    $ mkdir build
    $ cd build
    $ cmake ..
    $ make

## Run the program

Open a terminal in build directory and execute the following command:

    $ ./ZED\ Save\ depth [option]=[arg]

Example :

    $ ./ZED\ Save\ depth --resolution=3 --mode=2


## Options

               Option                    |               Descriptions             |                 Available Arguments                 |         Default Argument
-----------------------------------------|----------------------------------------|-----------------------------------------------------|------------------------------
 --help, -h , -?, --usage                | Display help message                   |                                                     |
 --filename                              | SVO filename                           | path to an SVO file                                 | <none>
 --path                                  | Output path                            | Output path                                         | ./
 --resolution                            | ZED Camera resolution (default 2)      | "0": HD2K, "1" : HD1080, "2" : HD720, "3" : VGA     | 2
 --quality                               | Disparity Map quality (default 2)      | "1": PERFORMANCE, "2": MEDIUM, "3": QUALITY         | 1
 --device                                | CUDA device                            | CUDA device                                         | -1

## Keyboard shortcuts

Hotkeys    |           Description                          
-------------|-----------------------------------
'p'         | Save the point cloud                                                          
'd'         | Save the depth image                                                                     
'm'         | Change point cloud file format        
'n'         | Change depth map file format        
'q'         | Exit the sample       
