Nirai's Panda3D
=======

Panda3D is a game engine, a framework for 3D rendering and game development for
Python and C++ programs.  Panda3D is open-source and free for any purpose,
including commercial ventures, thanks to its
[liberal license](https://www.panda3d.org/license.php).  To learn more about
Panda3D's capabilities, visit the [gallery](https://www.panda3d.org/gallery.php)
and the [feature list](https://www.panda3d.org/features.php).  To learn how to
use Panda3D, check the [documentation](https://www.panda3d.org/documentation.php)
resources. If you get stuck, ask for help from our active
[community](https://www.panda3d.org/community.php).

Panda3D is licensed under the Modified BSD License.  See the LICENSE file for
more details.

Building Panda3D
================

Windows
-------

We currently build using the Microsoft Visual C++ 2010 compiler.  You do not
need Microsoft Visual Studio to build Panda3D, though - the relevant compilers
are included as part of the Windows 7.1 SDK.

You will also need to have the third-party dependency libraries available for
the build scripts to use. These are available from the [third-party repository](https://github.com/nirai-compiler/thirdparty). Place the third-party directory into your Panda3D source directory.

After acquiring these dependencies, you may simply build Panda3D from the
command prompt using the following command:

```bash
compile.bat
postbuild.bat
```

_postbuild_ cleans up the _built_ dir.

Linux
-----

On Linux, you will need to obtain the relevant third-party dependencies for Nirai's Panda3D via means that your distro provides. You may visit [this manual page](https://www.panda3d.org/manual/index.php/Dependencies) for an overview of the various dependencies. 

If you are on Ubuntu, this command should cover the
third-party packages:

```bash
sudo apt-get install build-essential pkg-config python-dev libpng-dev libjpeg-dev libtiff-dev zlib1g-dev libssl-dev libx11-dev libgl1-mesa-dev libxrandr-dev libxxf86dga-dev libxcursor-dev bison flex libfreetype6-dev libvorbis-dev libeigen3-dev libopenal-dev libode-dev libbullet-dev nvidia-cg-toolkit libgtk2.0-dev
```

After acquiring the dependencies, you may simply build Panda3D from the terminal 
using the following command:

```bash
./compile.sh
./postbuild.sh
```

_postbuild_ cleans up the _built_ dir.

Mac OS X
--------

You will need to have the Mac OS X third-party dependencies available for 
the build scripts to use. These are available from the [third-party repository](https://github.com/nirai-compiler/thirdparty). Place the third-party directory into your Panda3D source directory. 

After acquiring these dependencies, you may simply build Panda3D from the terminal 
using the following command:

```bash
./compile.sh
./postbuild.sh
```

_postbuild_ cleans up the _built_ dir.
