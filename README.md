# opencv-deps

- cmake [github](https://github.com/Kitware/CMake) [homepage](https://cmake.org/)

   ```
   Uninstall old:

   sudo apt remove cmake
   
   sudo apt remove cmake-gui


   Install cmake:

   tar -zxvf cmake-3.22.0-rc1.tar.gz

   cd cmake-3.22.0-rc1/

   or:

   git clone https://github.com/Kitware/CMake

   cd CMake

   mkdir cmake-gui-build && cd cmake-gui-build

   sudo apt-get install -y libssl-dev build-essential

   sudo apt-get install -y qt5-default qtcreator 中间有一步安装qt5，如果你有qt了，你可以忽略这一步，但是qt要加入环境变量

   ../bootstrap --qt-gui && make -j 16 && sudo make install

   ```

- Eigen3 [gitlab](https://gitlab.com/libeigen/eigen)

- libjpeg (deprecated)  [homepage](http://www.ijg.org)

- libjpeg-turbo [github](https://github.com/libjpeg-turbo/libjpeg-turbo)

- libpng [homepage](http://www.libpng.org) [code](http://www.libpng.org/pub/png/libpng.html)

- libspng [homepage](https://libspng.org) [github](https://github.com/randy408/libspng/)

- libtiff [homepage](http://www.simplesystems.org/libtiff/) [gitlab](https://gitlab.com/libtiff/libtiff)

- zlib [homepage](http://www.zlib.net)

- jasper [github](https://github.com/jasper-software/jasper) [homepage](https://ece.engr.uvic.ca/~frodo/jasper/)

- openexr [homepage](http://www.openexr.com) [github](https://github.com/AcademySoftwareFoundation/openexr)

- ffmpeg [homepage](http://ffmpeg.org/)  [github](https://github.com/FFmpeg/FFmpeg)




---
## 如果出现编译错误

- error: ‘phase_unwrapping’ in namespace ‘cv’ does not name a type

  请参考网页 [Errors when compling the opencv_contrib on Ubuntu20.04 #3518](https://github.com/opencv/opencv_contrib/issues/3518)

  设置:
  
   CMAKE_INSTALL_PREFIX=/usr/local