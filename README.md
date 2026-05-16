# X-O

#use termminal UCRT64 /
pacman -Syu
# setup build tool
pacman-S mingw-w64-ucrt-x86_64-make \
        mingw-w64-ucrt-x86_64-cmake \
        mingw-w64-ucrt-x86_64-pkg-config
# setup SDL
pacman-S mingw-w64-ucrt-x86_64-SDL2 \
        mingw-w64-ucrt-x86_64-SDL2_image \
        mingw-w64-ucrt-x86_64-SDL2_ttf \
        mingw-w64-ucrt-x86_64-SDL2_mixer

# runfile at terminal level-2 folder to compile
mkdir build \
cd build \
cmake ..

# at build terminal run
cmake --build . \
to run in interactive mode: \
./game.exe \
to run in gui (graphic mode): \
./game.exe -g
