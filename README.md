FFmpeg README
=============

FFmpeg is a collection of libraries and tools to process multimedia content
such as audio, video, subtitles and related metadata.

## Libraries

* `libavcodec` provides implementation of a wider range of codecs.
* `libavformat` implements streaming protocols, container formats and basic I/O access.
* `libavutil` includes hashers, decompressors and miscellaneous utility functions.
* `libavfilter` provides a mean to alter decoded Audio and Video through chain of filters.
* `libavdevice` provides an abstraction to access capture and playback devices.
* `libswresample` implements audio mixing and resampling routines.
* `libswscale` implements color conversion and scaling routines.

## Tools

* [ffmpeg](http://ffmpeg.org/ffmpeg.html) is a command line toolbox to
  manipulate, convert and stream multimedia content.
* [ffplay](http://ffmpeg.org/ffplay.html) is a minimalistic multimedia player.
* [ffprobe](http://ffmpeg.org/ffprobe.html) is a simple analisys tool to inspect
  multimedia content.
* Additional small tools such as `aviocat`, `ismindex` and `qt-faststart`.

## Documentation

The offline documentation is available in the **doc/** directory.

The online documentation is available in the main [website](http://ffmpeg.org)
and in the [wiki](http://trac.ffmpeg.org).

### Examples

Coding examples are available in the **doc/examples** directory.

## License

FFmpeg codebase is mainly LGPL-licensed with optional components licensed under
GPL. Please refer to the LICENSE file for detailed information.

## DJI Build Script
DJI SDK uses FFmpeg as a static library (.so file). Our compiling processing is explained as follow:
### Android
The set-up :  MacBook Pro Mid 2015 15-inch,  running VMware Fusion Professional Version 8.5.6 (5234762), with image of ubuntu  ubuntu-16.04.2-desktop-amd64.iso 

* Edit the first line to match your NDK location.
* Find where `TOOLCHAINS_VERSION` was declared in the file and change it to your version. At this moment, DJI is using 4.9.
* Also change the PLATFORM_VERSION to the latest one that comes with your Android SDK. At this moment, DJI is using 21.
* To build the .so file of FFmpeg for Android, execute build_android.sh

### iOS
To build the .so file of FFmpeg for iOS, please execute build_iOS.sh

