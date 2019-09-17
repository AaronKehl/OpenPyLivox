# OpenPyLivox
Python3 driver for Livox lidar sensors

***Full documentation to follow soon!***

*NOTES:* 
- OpenPyLivox v1.0 has only been tested using Mid-40 sensors
- simultaneous operation of multiple Mid-40 sensors have been tested, but NOT using a Livox Hub
- the library has been tested on Mac OS X, Linux (GalliumOS on HP Chromebook), and Windows 10
- the library has been tested to work with Livox Mid-40 firmwares:
  - 03.03.0001 (double return)
  - 03.03.0002 (triple return)
  - 03.03.0003 (noise filtering)
  - 03.03.0004 (noise filtering - strict)
  - 03.03.0005 (short blind-zone)
  - 03.05.0000 to 03.06.0000 (standard versions)
- The CSV output file's header record allows the point cloud data to be easily opened in the <b>amazing</b> open source software, CloudCompare (download at https://cloudcompare.org)

```//X,Y,Z,Inten-sity,Time,ReturnNum      (ReturnNum is only included when using firmwares 03.03.0001 or .0002)```

*PYTHON DEPENDENCIES:*
```
crcmod     (used for computing the CRC16 and CRC32 request/response packet checks)
numpy      (currently used for simple math operations but future versions will heavily use np)
```


Check out the [livox_controller_demo.py](./livox_controller_demo.py) file for complete details on how to use the OpenPyLivox v1.0 library
