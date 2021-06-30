# ALTAIR
 




Building ALTAIR

On *nix


Dependencies: GCC 4.7.3 or later, CMake 2.8.6 or later, and Boost 1.55 or later, OpenSSL.

You may download them from:

    https://gcc.gnu.org/
    https://www.cmake.org/
    https://www.boost.org/
    https://www.openssl.org/

Alternatively, it may be possible to install them using a package manager.

To build, change to a directory where this file is located, and run make.

or

Run these commands:

cd ~

sudo apt-get install build-essential git cmake libboost-all-dev libssl-dev

git clone https://github.com/altair-coin/ALTAIR.git

cd ALTAIR

mkdir build

cd build

cmake ..

cd ..

make

The resulting executables can be found in build/release/src.

Advanced options:

    Parallel build: run make -j<number of threads> instead of make.
    Debug build: run make build-debug.
    Test suite: run make test-release to run tests in addition to building. Running make test-debug will do the same to the debug version.
    Building with Clang: it may be possible to use Clang instead of GCC, but this may not work everywhere. To build, run export CC=clang CXX=clang++ before running make.

On Windows

Dependencies: MSVC 2013 or later, CMake 2.8.6 or later, Boost 1.55 or later, OpenSSL. You may download them from:

    https://www.microsoft.com/
    https://www.cmake.org/
    https://www.boost.org/
    https://www.openssl.org/

To build, change to a directory where this file is located, and run these commands:

mkdir build
cd build
cmake -G "Visual Studio 15 Win64" ..

And then do Build. Good luck!
Building for macOS

Dependencies: cmake boost and Xcode

Download Xcode from the App store and the Xcode command line tools with xcode-select --install For the other we recommand you to use Homebrew

Continue with:

brew install git cmake boost
git clone https://github.com/altair-coin/ALTAIR.git
cd ALTAIR
cd build
cmake ..
make
