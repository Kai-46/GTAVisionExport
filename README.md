# GTAVisionExport
Basically, native/ and managed/ are both plugins for the game 'Grand Theft Auto V'. managed/ is based on native/.

For us, the really useful plugin is native/, I guess. Below, I'll briefly talk about how to compile it.

* Install Visual Studio 2019 Community edition; during installation, make sure to check Desktop development with C++ in the Workloads page.

* clone this repo

* open Developer Command Prompt for VS 2019

* cd {path to GTAVisionExport}/native

* mkdir build && cd build

* cmake -DEIGEN3_INCLUDE_DIR=../../eigen -G "Visual Studio 16 2019" -A x64 ..

* now you will see 'GTANativePlugin.sln' in build/; double click to open it in VS 2019

* in VS 2019, click Build -> Build Solution

* you will see the plugin file as build/src/Debug/GTAVisionNative.asi
