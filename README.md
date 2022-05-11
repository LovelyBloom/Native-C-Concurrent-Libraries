# Native C concurrent Libraries
This repo is aimed at briging multithreading and async i/o to C

THIS RESEARCH IS IN NO WAY A NEW C LANGUAGE OR AN EXTENSION OR A FORK OF IT.

THE REPO WILL USE AGILE PROGRAMMING STANDARDS, DOXYGEN AND COMMITS MUST BE TEST COMPATIBLE OR WON'T BE MERGED

we have a that cockroach inside our computer's C Language if we open it and we're here to remove it. 

As we Speak in the Realm of C/C++ Programming, There is no offically complete native concurrent library for C
the best approach to a bug-free program is to still using the old C Version wiht pthreads, and as for C++ the confident option is still C++17 with asyinc features in the <future> include

C programmers use pthreads a Posix Standard multithreading library, the most complete concurrent library (with the newer asynchronous I/O model nowhere
to be found.). The posix threading library is fully optimized against the linux and unitx-like kernels taking advantages of features available for concurrent accuracy
and proper functionality. with most developer moving their code to win32 the mere attempt to to cross-platform this issue is supplement the executable with mingw-w64's dlls that
dump all the kernel fuctionalities and pseudo run a concurrent executable (that if you investigate by running simple tests, [you'd be surprised by the results](https://pastebin.com/xDWEBusA).

clearly only a ucrt that compiles against the proper windows sdk can deliver true concurency to windows with kernel support. and that's where our native library's abis come in.
having the same advantage a posix one has, yet there's no unified native library of this sort.

so our library depending on the operating system will use the proper requirements such as proper windows sdk for windows.

and since we want it everywhere we'll use the llvm's infrastructure. compiling with clang and clang-cl

we are in need of the two current concurrent models: Multi-Threading And Asynchronous I/O. Study of Python 3.8+ of their implementation will help us with those.
and we can use visual studio's clang compiler, ucrt and llvm's feature rich assembly output of various - from most easy to read to most assembly pure - to help us with
analysing our progress.

The first commit of this research might surprise you as I (Almost) always use Pseudo-Python3 codes for my first drafts.
and it might turn into an attempt at a new cross-native compiler (Since my latest Ivor Horton's Edition on C++ Still doesn't compile and 23 is upon us) with the library in maintained in a different repo. so I'll start the theoretical studies part of this repo/research.

SO UNTIL THE FIRST COMMIT. STAY FROSTY
