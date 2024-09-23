# ashbaugh_plugin
Component (plugin) for HOOMD-blue version 3 with Ashbaugh-Hatch pair potential.
Currently, it is tested against v3.8.1 of HOOMD-blue

## Compilation
ashbaugh_plugin can be compiled as an **external** component following the standard HOOMD-blue methods (visit [hoomd documentation](https://hoomd-blue.readthedocs.io/en/v3.8.1/components.html)) 

Ensure that the hoomd module is on your Python path (or hint to its location using HOOMD_ROOT), and install to an appropriate location:

```
cd /path/to/ashbaugh_plugin
mkdir build && cd build
cmake ..
make install

You must make sure that your installation location is on your PYTHONPATH, and then ashbaugh_plugin can be imported as usual:

```python
  import hoomd
  import azplugins

## Prerequisites
ashbaugh_plugin requires the same dependencies used to build HOOMD-blue. Typically, this means a modern Python installation with numpy, a reasonably recent version of CMake, and a C++11 capable compiler. To get good performance, you probably also want a recent CUDA toolkit and an MPI library.

