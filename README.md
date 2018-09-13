This project serves as a starting point of high speed image processing and display results asynchronously.

High speed image processing is done in worker thread. 
Displaying process is done asynchronously irrerevelant to the state of working thread.

Some remarks:
- In compatible with modern C++ compiler (that supports C++11)

- No additinoal library required. No Boost, No Qt.

- Primarily designed for CLion and Mac, but should work with other IDEs and operating system.

- You should add paths before compile. For ease of use, here is excerpt from my .bash_profile
```
# OpenCV
export OpenCV_DIR=/Users/mhirano/opencv-3.2.0/build
export OpenCV_LIBS=/Users/mhirano/opencv-3.2.0/build/lib
export OpenCV_INCLUDE_DIRS=/Users/mhirano/opencv-3.2.0/include
```
Otherwise, set environmental variable in CMakeLists.txt as directed within the file.

- Use out-of-source build. Namely, run cmake within debug/release directory as `cmake ..`
