# Stage 2

Here, we introduce the ```Program``` builder for building C++ program.

### Binary

To build this example you cd to directory containing SConstruct file and execute,
```
scons
```

If the build is successful, Scons prints the following output:

```
$ scons 
scons: Reading SConscript files ...
scons: done reading SConscript files.
scons: Building targets ...
g++ -o hello-greet.o -c -Ih hello-greet.cc
g++ -o hello-world.o -c -Ih hello-world.cc
g++ -o hello-world hello-world.o hello-greet.o
scons: done building targets.

```
In the run log above you can see where the executable was built.
