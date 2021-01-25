# Stage 3

In this stage we step it up and showcase how to integrate sources in multiple directories

The SConstruct file lists the SConscript files to be executed.

To use our ```hello-time``` libary, Scons environment is used.

To build this example you cd to directory containing SConstruct file and execute,
```
scons
```

If the build is successful, Scons prints the following output:

```
scons: Reading SConscript files ...
scons: done reading SConscript files.
scons: Building targets ...
g++ -o lib/hello-time.o -c lib/hello-time.cc
ar rc lib/libhello-time.a lib/hello-time.o
ranlib lib/libhello-time.a
g++ -o main/hello-greet.o -c -Ilib main/hello-greet.cc
g++ -o main/hello-world.o -c -Ilib main/hello-world.cc
g++ -o main/hello-world main/hello-greet.o main/hello-world.o -Llib -lhello-time
scons: done building targets.

```
The log shows the location of the final executable.
