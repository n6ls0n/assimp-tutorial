# Assimp Tutorial

## Table of Contents

- [Introduction](#introduction)
- [Installation Steps](#installation-steps)
- [Project Use](#project-use)
- [References](#references)

### Introduction

This is a short tutorial on how to build Assimp from source on Windows on VS Code and then use it within a project without installing it directly on your system.

You can also install using vcpkg but make sure you run the .bat files of the same name

### Installation Steps

- Download the latest source code release from the GitHub Repo (2)

- Extract to a directory of the same name from here on referred to as {extracted base folder}

- cd into the new directory

- create a new build directory

- cd into the build directory

- run "cmake .."

- open the resultant .sln file in the build directory

- Build the "ALL_BUILD" solution

- The resultant build files consist of a .lib and a .dll file. They can be found at the following locations:
    1. {extracted base folder}\build\lib\Debug\assimp-vc143-mtd.lib
    2. {extracted base folder}\build\bin\Debug\assimp-vc143-mtd.dll

- To use within a project, you will also need to copy the "include" folder in the {extracted base folder}

### Project Use

To demonstrate how to use Assimp within a project, we will build a model loader & viewer.
This project is based on an example from the learn-opengl book (3).
A huge thank you to Joey De Vries(<https://joeydevries.com/#home>).

To run the example:

  1. Ensure you have Visual Studio installed
  2. Navigate to Model Loading/ and run the build_run_project.bat file

### References

1. Build Instructions - <https://github.com/assimp/assimp/blob/master/Build.md>

2. Github Repo - <https://github.com/assimp/assimp/tree/master>

3. Learn OpenGL Book - <https://learnopengl.com/>
