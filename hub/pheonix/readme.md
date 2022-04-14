

# Get Started with development
### Setup Compiler

Need gcc to be 10 to support coroutines and c++20. Why not clang? because pytorch is compiled using gcc so for now we will use gcc-10
```
sudo apt install gcc-10 g++-10
```
then point c++ to gcc-10

```
sudo update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-10 1000 --slave /usr/bin/g++ g++ /usr/bin/g++-10
```

### Install Scheduler

Install boost asio
```
wget https://boostorg.jfrog.io/artifactory/main/release/1.78.0/source/boost_1_78_0.tar.gz
tar -zxvf boost_1_78_0.tar.gz
```


update bashrc
```
export PATH=$PATH:/Users/levongh/Downloads/boost_1_78_0
export DYLD_LIBRARY_PATH=$DYLD_LIBRARY_PATH:/Users/levongh/Downloads/boost_1_78_0/stage/lib
```

example https://github.com/jgaa/asio-composed-blog/blob/main/echo-server.cpp

### Package manager
- [] try hunter gate


