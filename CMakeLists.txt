
# CMake4FPGA
# This is the first example of the CMake4FPGA tutorial that will teach you how to use CMake 
# for FPGA design and perform a full version control over GitHub
#
#
# Author : Mostafa Darvishi, Ph.D.
#          Digital Electronics|Hardware Design|FPGA Developer
 

# first, you should specify the Python version to be used by CMakeLists.txt file
# second, name your project (i.e. helloworld here)
cmake_minimum_required(VERSION 3.3)
project(helloworld)

#force the programer to build the make files out of the source file directory specifically
# in a build directory make by mkdir command
set(CMAKE_DISABLE_SOURCE_CHANGES ON)
set(CMAKE_DISABLE_IN_SOURCE_BUILD ON)

#defines variable mymessage and then check its status to print out the result of make process
set(mymessage "Hello World! Welcome to CMake4FPGA...")
message(STATUS ${mymessage})
