# C-Tutorial-Demos
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


