# Fast Bitmap Rotation Library

**Target platform:** Android

**Algorithms:** Currently only 180 degrees rotations are supported.

**Limitations:** Only in place rotations (without allocating additional memory).

**Implementation:** C++ library for Java.

**Applications:** Useful for camera applications.


#### Performance (approximately)
* 5 times faster than Matrix rotation method.
* 3.8 times faster than Ndk rotation method.
* 3.3 times faster than OpenCV rotation method.

#### How to run the application and check performance
Clone the project, open it in Android Studio and run.
Wait approximately 20 seconds and the results will be on the screen.

#### How to use the library in your project
* Add the following line: `include ':fast_bitmap_rotation_lib'` to `settings.graddle` file.
* Add the following line: `implementation project(':fast_bitmap_rotation_lib')` to `dependencies` section of application `build.gradle` file.

#### Acknowledgments
* [riwnodennyk](https://stackoverflow.com/users/986216/riwnodennyk "riwnodennyk") - idea and different rotation implementations.
* A [discussion](https://stackoverflow.com/a/29734593/1707617) on different rotation methods.
* GitHub [repository](https://github.com/riwnodennyk/ImageRotation) with different rotation methods.
* [Ndk](https://developer.android.com/ndk) - a toolset that lets you implement parts of your app in native code, using languages such as C and C++.
* [Description](https://stackoverflow.com/questions/72251642/super-fast-bitmap-180-degrees-rotation-using-opencv-on-android) of OpenCV implementation.
