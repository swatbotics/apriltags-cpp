apriltags-cpp
=============

C++ port of the APRIL tags library, using OpenCV (and optionally, CGAL).

Requirements
============

Currently, apriltags-cpp requires the following to build:

  * OpenCV >= 2.3
  * GLUT or freeglut (optional, used for test program)
  * Cairo (optional, used to print tags)
  * CGAL (optional, used for new quad detection algorithm)

You must have cmake installed to build the software as well.

Building
========

To compile the code, 

    cd /path/to/apriltags-cpp
    mkdir build
    cd build
    cmake .. -DCMAKE_BUILD_TYPE=Release
    make

Demo/utility programs
=====================

The APRIL tags library is intended to be used as a library, from C++,
but there are also five demo/utility programs included in this
distribution:

   *   `tagtest` - Demonstrate tag recognition and time profiling. 
     
   *   `camtest` - Demonstrate 3D tag locations using OpenCV to
       visualize, with an attached camera.

   *   `gltest` - Demonstrate 3D tag locations using OpenGL to
       visualize, with an attached camera.

   *   `quadtest` - Demonstrate/test tag position refinement using
       a template tracking approach.

   *   `maketags` - Create PDF files for printing tags.

There are some test images in the `images` directory, that may be
useful to use with the `tagtest` program.
