# AMDVideoCrashReproducer

This sample reproduces a crash in a producer/consumer scenario with YUV420 video frames. The program consists of a producer that continuously populates a shared texture array with video frames in a producer thread. The content of this texture array is displayed in a window on the main thread.

When running this code on an AMD GPU, the program crashes because the Direct3D device is lost. On NVidia and Intel, the program runs as expected, showing a flickering colored image.

![image](https://github.com/jogerh/AMDVideoCrashReproducer/assets/16581681/22f195df-b4e9-4c46-82c7-4010d5d3e179)
