# zed-save-depth

**This sample is designed to work with the ZED stereo camera only and requires the ZED SDK. For more information: https://www.stereolabs.com**

This sample allows you to save depth information provided by the ZED Camera or by an SVO file, in different formats (PNG 16-Bit, PFM, PGM, XYZ, PCD, PLY, VTK).

This sample requires OpenCV and Boost (program_options).

##Build the program

Open a terminal and execute the following command:

    $ mkdir build
    $ cd build
    $ cmake ..
    $ make

##Run the program

Open a terminal in build directory and execute the following command:

    $ ./ZED\ Save\ depth [option] [arg]
    

##Options
 
               Option                    |            Descriptions                |         Argument     
-----------------------------------------|----------------------------------------|---------------------------------------
 --help                                  | Display help message                   |
 -f, --filename                          | SVO filename                           | path to an SVO file
 -p, --path                              | Output path                            | string
 -r, --resolution                        | ZED Camera resolution (default 2)      | "0": HD2K, "1" : HD1080, "2" : HD720, "3" : VGA
 -q, --quality                           | Disparity Map quality (default 2)      | "1": PERFORMANCE, "2": QUALITY
 -d, --device                            | CUDA device                            | int
