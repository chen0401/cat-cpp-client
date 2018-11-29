# cat-cpp-client
# Environment
- cat 3.0.0
- g++ 4.8.0
- CentOS 6
# Download CAT and save as /home/cat-master
```
git clone https://github.com/dianping/cat
```
# compile
```
mkdir cmake
cd cmake
cmake ..
make
```
# Demo
```
mkdir -p {include/cat,libs,src}
cp /home/cat-master/lib/cpp/include/client.hpp include/cat
cp /home/cat-master/lib/cpp/cmake/libcatclient.so libs
```
## main.cpp
## Makefile
###
```
make
./catcpp
```
