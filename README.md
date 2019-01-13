# Approximate-computing-on-Neural-Networks
Evaluating the impact of weighs accuracy reduction in a Neural Network over the Classification Accuracy

The amount of memory used to store the parameters of a neural network is dominated by storing weights. Therefore, reducing the number of bits to represent weights has a positive impact on use on the amount of resources required. The reduction in the number of bits also offers the possibility of using reduced arithmetic circuits with a consequent reduction in area, power and possibly a reduction in the critical path and therefore an increase in the clock frequency. The reduction in the number of bits used to represent weights certainly has an impact on the accuracy of the neural network. We want to evaluate this impact.

## Table of Contents

- [References](#references)
- [Screenshots](#screenshots)
- [Requirements](#requirements)
- [Dependencies](#dependencies)
- [Testing](#running-for-test)



## References

References available (italian only) at:
- doc/Relazione_Scavo_Messina.docx



## Screenshots

Not yet available


## Requirements

- Cmake
- Visual Studio (2015 or successive versions) with c++ compiler installed


## Dependencies

- tiny-dnn (repo: https://github.com/tiny-dnn/tiny-dnn)


## Running for Test
You can clone this project and run it following the next steps

#### 1 - Clone the project from develop branch
- Start Command Prompt window (cmd.exe).
- On the command line, write
  - ```bash git clone https://github.com/Taletex/Approximate-computing-on-Neural-Networks.git ```

#### 2 - Build the project for Visual Studio
- Start Command Prompt window (cmd.exe). 
- On the command line, write
  - ```bash mkdir build ``` (Make build folder at the project path)
  - ```bash cd build ``` (Set current directory to the folder)
- Then you need to generate projects with below command (don't forget to delete CMakeCache.txt prior to running the command.)
  - Visual Studio 2015
    - 32bit : cmake -G "Visual Studio 14 2015" -DBUILD_EXAMPLES=ON ..
    - 64bit : cmake -G "Visual Studio 14 2015 Win64" -DBUILD_EXAMPLES=ON ..
  - Visual Studio 2017
    - 32bit : cmake -G "Visual Studio 15 2017" -DBUILD_EXAMPLES=ON ..
    - 64bit : cmake -G "Visual Studio 15 2017 Win64" -DBUILD_EXAMPLES=ON ..
- Open tiny_dnn.sln file (located in build directory) with Visual Studio.
- Build Solution (F7)


#### 3 - Run the project
On Visual Studio (after compilation is done) you can delete all project except from the ac_nn one (you can also leave them, but if you do it you need to set the ac_nn project as the starting project). Then you can run the project simply by use "debug" or "run without debug" buttons.
