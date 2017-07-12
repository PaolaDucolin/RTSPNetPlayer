WebEye is a collection of .NET controls. So far, the collection consists of two controls:

1. StreamPlayerControl is a FFmpeg-based stream player control
2. WebCameraControl is a DirectShow-based web camera control 

The controls are simple and easy to use, have no additional dependencies and a minimalistic interface.

Requirements:
 > Boost: 
   1. Download boost from http://www.boost.org/users/history/version_1_64_0.html
   2. Extract to a folder and cd in it
   3. For VisualStudio 2013 64bit, run #bjam --toolset=msvc-12.0 address-model=64 --build-type=complete
   4. Add bin/include/boost-1_64 to StreamPlayer include path
   5. Add stage/lib to StreamPlayer library path
 > FFMPEG:
   1. Clone FFMPEG git repository https://github.com/FFmpeg/FFmpeg.git, and checkout last tagged release
   2. For VisualStudio 2013 64bit, run #./configure --toolchain=msvc --arch=amd64 --target-os=win64 --enable-version3 --enable-static --disable-shared --disable-programs --disable-doc --prefix=<ffmpeg_output_path>
   3. Add <prefix_output_path>/include to StreamPlayer include path
   4. Add <prefix_output_path>/lib to StreamPlayer library path
