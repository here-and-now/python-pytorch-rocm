What a strange journey it has been ...


1. use arch4edu repo
2. pacman -S rocm-hip-sdk rocm-opencl-sdk
3. check hipmagma
4. libfmt.so.8 needed, build with installation instructions from https://fmt.dev/latest/usage.html#building-the-library, build shared libs important

mkdir build          # Create a directory to hold the build output.
cd build
cmake ..  # Generate native build scripts.
cmake -DBUILD_SHARED_LIBS=TRUE

5. move or install the shared library to /usr/lib/


