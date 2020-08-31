## OpenCV: Open Source Computer Vision Library

This fork contains Delicode's projectPoints3d functionality and a timeout in findChessboardCorners.

If you're building OpenCV on a Linux computer targeting the Delicode Signals software stack, you'll want to use a CMake command along these lines:

```
cmake -DWITH_CUDA=no -DBUILD_TESTS=OFF -DBUILD_PERF_TESTS=OFF -DBUILD_EXAMPLES=OFF -DBUILD_DOCS=OFF -DOPENCV_EXTRA_MODULES_PATH=/path/to/opencv_contrib/modules -DBUILD_opencv_aruco=ON .. 
```

Note you'll need `https://github.com/opencv/opencv_contrib` cloned into a path specified above. At the time of writing, this repo uses OpenCV 4.1.2, which is also the tag you *must* checkout in the `opencv_contrib` repo by issuing: `git checkout 4.1.2`. The two repos must use the same release tag.

### Resources

* Homepage: <https://opencv.org>
* Docs: <https://docs.opencv.org/master/>
* Q&A forum: <http://answers.opencv.org>
* Issue tracking: <https://github.com/opencv/opencv/issues>

### Contributing

Please read the [contribution guidelines](https://github.com/opencv/opencv/wiki/How_to_contribute) before starting work on a pull request.

#### Summary of the guidelines:

* One pull request per issue;
* Choose the right base branch;
* Include tests and documentation;
* Clean up "oops" commits before submitting;
* Follow the [coding style guide](https://github.com/opencv/opencv/wiki/Coding_Style_Guide).
