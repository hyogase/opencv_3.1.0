### OpenCV: Open Source Computer Vision Library
Kai LU

[![Gittip](http://img.shields.io/gittip/OpenCV.png)](https://www.gittip.com/OpenCV/)

#### Resources

* Homepage: <http://opencv.org>
* Docs: <http://docs.opencv.org/master/>
* Q&A forum: <http://answers.opencv.org>
* Issue tracking: <https://github.com/Itseez/opencv/issues>

#### Contributing

Please read before starting work on a pull request: <https://github.com/Itseez/opencv/wiki/How_to_contribute>

Summary of guidelines:

* One pull request per issue;
* Choose the right base branch;
* Include tests and documentation;
* Clean up "oops" commits before submitting;
* Follow the coding style guide.

LINK : warning LNK4044: 无法识别的选项“/LC:/Program Files/NVIDIA GPU Computing Toolkit/CUDA/v8.0/lib/x64”；已忽略
http://blog.csdn.net/github_32886825/article/details/53354090
http://stackoverflow.com/questions/36317625/opencv-wont-build-with-cuda-even-though-with-cuda-on-in-cmake

D:\opencv\opencv-3.1.0\CMakeLists.txt
  foreach(p ${CUDA_LIBS_PATH})
#    set(OPENCV_LINKER_LIBS ${OPENCV_LINKER_LIBS} -L${p})
     set(OPENCV_LINKER_LIBS ${OPENCV_LINKER_LIBS} ${CMAKE_LIBRARY_PATH_FLAG}${p})
  endforeach()
