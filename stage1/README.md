# Stage 1

This example shows how to build a single file to create a runnable application.

This SConstruct file shows that we want to build a C++ binary using the ```Program``` builder provided by Scons.

To build this example you cd to directory containing SConstruct file and execute,
```
scons
```

If the build is successful, Scons prints the following output:
```
scons: Reading SConscript files ...
scons: done reading SConscript files.
scons: Building targets ...
g++ -o hello-world.o -c hello-world.cc
g++ -o hello-world hello-world.o
scons: done building targets.
```

In the run log above you can see where the executable was built so you can execute it.
