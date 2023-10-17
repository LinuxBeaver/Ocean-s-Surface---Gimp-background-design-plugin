Download binaries here. (FOLLOW INSTRUCTIONS)

https://github.com/LinuxBeaver/Ocean-s-Surface---Gimp-background-design-plugin/releases/tag/Ocean_Surface_gimp_plugin_for_background_design

# Ocean's surface - Gimp plugin for background design.
![image](https://github.com/LinuxBeaver/Ocean-s-Surface---Gimp-background-design-plugin/assets/78667207/ae127e44-8f4f-4560-9edc-d970a45e2da4)


## OS specific location to put GEGL Filter binaries 

**Windows**
C:\Users\USERNAME\AppData\Local\gegl-0.4\plug-ins
 
** Linux **
 /home/(USERNAME)/.local/share/gegl-0.4/plug-ins
 
 **Linux (Flatpak)**
 /home/(USERNAME)/.var/app/org.gimp.GIMP/data/gegl-0.4/plug-ins

![image](https://github.com/LinuxBeaver/GEGL-glossy-balloon-text-styling/assets/78667207/f15fb5eb-c8d7-4c08-bbac-97048864e657)

Then Restart Gimp and go to GEGL operations and look for "ocean surface" if you have Gimp 2.99.16+ you will find this in filters>render>fun

## Compiling and Installing
**Linux**

To compile and install you will need the GEGL header files (libgegl-dev on Debian based distributions or gegl on Arch Linux) and meson (meson on most distributions).

meson setup --buildtype=release build
ninja -C build


If you have an older version of gegl you may need to copy to ~/.local/share/gegl-0.3/plug-ins instead (on Ubuntu 18.04 for example).

**Windows**

The easiest way to compile this project on Windows is by using msys2. Download and install it from here: https://www.msys2.org/

Open a msys2 terminal with C:\msys64\mingw64.exe. Run the following to install required build dependencies:

pacman --noconfirm -S base-devel mingw-w64-x86_64-toolchain mingw-w64-x86_64-meson mingw-w64-x86_64-gegl

Then build the same way you would on Linux:

meson setup --buildtype=release build
ninja -C build

## Extra preview of this based Gimp plugin
![image](https://github.com/LinuxBeaver/Ocean-s-Surface---Gimp-background-design-plugin/assets/78667207/ffd0210a-94dc-4bc1-a2a6-c8b61a9bf632)

