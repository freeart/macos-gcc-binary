# GCC 8.2 binary for macOS 10.14 Mojave #

This is the macOS binary for the current stable release of *GCC 8.2*, this file is provided for your convenience, if you prefer to compile it yourself visit the tutorial webpage for build instructions:

[https://solarianprogrammer.com/2017/05/21/compiling-gcc-macos/](https://solarianprogrammer.com/2017/05/21/compiling-gcc-macos/)

How to use:
===========

Get the binary:

```console
curl -L https://github.com/sol-prog/macos-gcc-binary/releases/download/gcc-8.2.0/gcc-8.2-macos-mojave.tar.xz | tar xf -
```

In order to install this binary extract gcc-8.2-macos-mojave.tar.xz and copy the extracted folder (gcc-8.2) to your /usr/local folder.

```console
tar xf gcc-8.2-macos-mojave.tar.xz
sudo mv gcc-8.2 /usr/local

echo 'export PATH=/usr/local/gcc-8.2/bin:$PATH' >> ~/.bash_profile
source ~/.bash_profile
```

Compiling a C++17 code is as simple as:

g++-8.2 -std=c++17 file_name.cpp -o file_name:

If you need more help leave me a comment at:

[https://solarianprogrammer.com/2017/05/21/compiling-gcc-macos/](https://solarianprogrammer.com/2017/05/21/compiling-gcc-macos/)
