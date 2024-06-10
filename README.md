# eigen-cddlib

Eigen wrapper for Komei Fukuda's [cdd](https://www.inf.ethz.ch/personal/fukudak/cdd_home/) library.

## Installing

First install ``cddlib``:
```sh
sudo apt-get install libcdd-dev
```
Then, install ``eigen-cddlib`` following the standard CMake procedure:

```sh
git clone --recursive https://github.com/philip-long/eigen-cddlib
cd eigen-cddlib
mkdir build
cd build
cmake .. -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFX:='your_path_ws/src/eigen-cddlib/build/'
make -j4
sudo make install
```
<your_path>- refers to the build folder created in the workspace
If cdd has not been installed in the default path, CMake may not find it. In this case, add the path as a HINTS in ``find_path`` and/or ``find_library``.

### Testing

```sh
cd eigen-cddlib/build
make test
```

## Examples

There is no basic examples yet. Please see test files for an overview, and doxygen files for API documentation.
