# Cplusplus-Tutorial-Demos
Reference code for cool, weird, or new features of C++ for demonstration purposes

This repository has grown organically as I add codes to experiment due to requests from students, curiousity, or the need to puzzle out code found online or in projects.

A frequent pattern to them is that, since we are trying to understand not only behavior, but what is allowed, they contain code that works as well as commented code that does not work. For example:

```c++
class SimpleClass {
        int x;
};

struct SimpleStruct {
        int x;
};

int main(int argc, char**argv) {
        // Default accessibility:
        SimpleClass moo;
        // Class defaults to private    
        // moo.x = 0;
        SimpleStruct noo;
        noo.x = 0;
}
```

Note that in the code above, the comment //moo.x=0 is just as important to the lesson, being that struct members are public by default while class members are public by default.

Compilation should work on the command line on Linux or Mac. It may work on a Windows installation with Visual Studio installed using NMake.

```
$ ls Makefile 
Makefile
$ make clean
rm -f abstract ...
$ make
c++ -o accessors_mutators accessors_mutators.cpp
$ ./accessors_mutators 
10
10
```

Ready for the codes? OK, here we go! :bowtie:

* abstract.cpp Lessons in abstract classes, their children, and references.
   Failing to define a function results in an error, unless it is a pure virtual function, which results in an abstract class. Abstract classes must not be initialized, though you can hold references to their children using the abstract parent types. This is, in fact, the purpose of abstract classes
        


