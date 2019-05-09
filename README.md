# GCC 9.1 binary for macOS 10.14 Mojave #

This is the macOS binary for the current stable release of *GCC 9.1*, this file is provided for your convenience, if you prefer to compile it yourself visit the tutorial webpage for build instructions:

[https://solarianprogrammer.com/2017/05/21/compiling-gcc-macos/](https://solarianprogrammer.com/2017/05/21/compiling-gcc-macos/)

How to use:
===========

Get the binary and extract the archive:

```bash
curl -L https://github.com/sol-prog/macos-gcc-binary/releases/download/v9.1/gcc-9.1-macos-10.14.tar.bz2 | tar xf -
```

In order to *install* the compiler copy gcc-9.1 to your /usr/local folder.

```bash
sudo mv gcc-9.1 /usr/local

echo 'export PATH=/usr/local/gcc-9.1/bin:$PATH' >> ~/.bash_profile
source ~/.bash_profile
```

Compiling a C++17 code is as simple as:

g++-9.1 -std=c++17 file_name.cpp -o file_name:

If you get an error about missing headers

```bash
cd /Library/Developer/CommandLineTools/Packages/
open .
```

If you need more help leave me a comment at:

[https://solarianprogrammer.com/2017/05/21/compiling-gcc-macos/](https://solarianprogrammer.com/2017/05/21/compiling-gcc-macos/)
