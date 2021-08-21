# cmake_examples  


## project structure  

cmake_test/  
├── CMakeLists.txt  
├── build  
├── cmake_test.cpp  
└── studentLibrary  
&nbsp;&nbsp;&nbsp;&nbsp;├── CMakeLists.txt  
&nbsp;&nbsp;&nbsp;&nbsp;├── build  
&nbsp;&nbsp;&nbsp;&nbsp;├── include  
&nbsp;&nbsp;&nbsp;&nbsp;│   └── Student.h  
&nbsp;&nbsp;&nbsp;&nbsp;└── src  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└── Student.cpp  

5 directories, 5 files  

## buid inner project  

$ cd studentLibrary  
$ cd build  
$ cmake ..  
$ make  

  this will generate the shared library inside the build folder  
  
$ sudo make install  

  this will push the shared library into /usr/lib location  
  

## build outer project  


$ cd cmake_test  
$ cd build  
$ cmake ..  
$ make  

  this will build the executable file in the build folder  
  
## run the executable  

$ ./libtest
