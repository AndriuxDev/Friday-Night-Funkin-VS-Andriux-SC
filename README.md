# Friday-Night-Funkin-VS-Andriux-SC

![fnf+andy](https://user-images.githubusercontent.com/86565812/123558237-ce1d7e80-d75a-11eb-8ff7-d36f32a1f49f.png)

## History
Andriux is on his way to find the truth behind his own life. However, Boyfriend, Monika and Senpai will make their way towards his soul to make him realize he can be happy. Will the sadness prevail, or will there be heroes to the rescue?

## How to help with the mod
This mod is still in development, but you can collaborate and send your progress to the creator!

# Installing the Required Programs
First you need to install Haxe and HaxeFlixel.
1.	Install Haxe 4.1.5 (Download 4.1.5 instead of 4.2.0 because 4.2.0 is broken and is not working with gits properly...)
2.	Install HaxeFlixel after downloading Haxe.
Other installations you will need are the additional libraries. A fully updated list will be in Project.xml in the project root. Currently, these are all the things you need to install:
flixel
flixel-addons
flixel-ui
hscript
newgrounds

So, for each of those type **haxelib install library** so shit like haxelib install newgrounds.
You will also need to install a couple things that involve Gits. To do this, you need to do a few things first:

1.	Download **git-scm**. Works for Windows, Mac, and Linux, just select your build.
2.	Follow instructions to install the application properly.
3.	Run haxelib git polymod https://github.com/larsiusprime/polymod.git to install Polymod.
4.	Run haxelib git discord_rpc https://github.com/Aidan63/linc_discord-rpc to install Discord RPC.
5.	Optional: - Run haxelib git flixel-addons https://github.com/HaxeFlixel/flixel-addons to update Flixel-Addons. This fixes the transition bug for zoomed out stage cameras.

You should have everything ready for compiling the mod! Follow the guide below to continue!

# Adding APIStuff.hx into /source
The API keys of the mod were git-ignored so no one could post fake high scores onto the leaderboards in Newgrounds. Unfortunately, because this mod requires the API and EncKey values to compile, you will need to add a file called APIStuff.hx into /source.

1.	Create a new text file called APIStuff.hx inside of the /source folder.
2.	Copy the following text:
```
package;
class APIStuff
{
	public static var API:String = "";
	public static var EncKey:String = "";
}
```
3.	Paste the text into the APIStuff.hx file and save the file.
You should be good from there! Now, onto compiling!
Compiling the Mod

# Desktop Building:
Desktop building can be a bit tedious. Each different version requires a different setup.

## Linux Building:
1.	Open your machine's command prompt/terminal and navigate to your root folder of the mod. An easy guide can be found here [https://ninjamuffin99.newgrounds.com/news/post/1090480]!
2.	Type *lime build linux -debug* to build the Linux version of the mod.
3.	Type *lime run linux -debug* to run the Linux version of the mod from the command prompt/terminal. (You can also run the mod from funkin/export/debug/linux/bin)

## Mac Building:
1.	Open your machine's command prompt/terminal and navigate to your root folder of the mod. An easy guide can be found here [https://ninjamuffin99.newgrounds.com/news/post/1090480]!
2.	Type *lime build mac -debug* to build the Mac version of the mod.
3.	Type *lime run mac -debug* to run the Mac version of the mod from the command prompt/terminal. (You can also run the mod from funkin/export/debug/mac/bin)

## Windows Building:
THIS METHOD REQUIRES AROUND 22 GIGABYTES OF STORAGE.
1.	Install Visual Studio Community 2019 [https://visualstudio.microsoft.com/downloads/].
2.	Open the installer and go to the individual workloads tab and download the following:

* C++ CMake tools for windows 
*	C++ Profiling tools 
*	C++ ATL for v142 build tools (x86 & x64)
*	C++ MFC for v142 build tools (x86 & x64)
*	C++/CLI support for v142 build tools (14.21)
*	C++ Modules for v142 build tools (x64/x86)
*	Clang Compiler for Windows
*	MSVC v140 - VS 2015 C++ build tools (v14.00) 
*	MSVC v141 - VS 2017 C++ x64/x86 build tools
*	MSVC v142 - VS 2019 C++ x64/x86 build tools
*	Windows 10 SDK (10.0.16299.0)
*	Windows 10 SDK (10.0.17134.0)
*	Windows SDK (10.0.17763.0)

3.	Wait for the install to finish, which might take a while.
4.	Open your machine's command prompt/terminal and navigate to your root folder of the mod. An easy guide can be found here [https://ninjamuffin99.newgrounds.com/news/post/1090480]!
5.	Once everything is installed, type *lime build windows -debug* to build the windows version of the mod.
6.	Type *lime run windows -debug* after the mod is compiled to run the windows version of the mod. (You can also run the mod from funkin/export/debug/windows/bin)

