Wisp Building from source for Windows (WISP)
====================================================


Install MSVC 2017 and Qt SDK (Pick MSVC 64 bit and QtWebEngine)
------------

- Visual studio: https://www.visualstudio.com/downloads/
- Qt SDK: https://www.qt.io/download-qt-installer

Here is the components from Qt SDK that we really need to compile our application (Keep Qt creator selected as well). If MingW is ticked you may untick that (Unless you need it for other projects)

![alt text](https://github.com/spectrecoin/spectre/raw/master/doc/Qt%20windows.png)

Once you install Visual studio. Go to Windows start menu and find "Visual studio installer"

Modify visual studio and make sure all those components are picked.

![alt text](https://github.com/spectrecoin/spectre/raw/master/doc/Visual%20studio%20installer%20components.png)



Easy (Prebuilt libs)
--------------------

Since quit many of our users found it hard to compile. Especially on Windows. We are adding an easy way and provided prebuilt package for all the libraries required to compile Wisp wallet. Go ahead and download all the libraries from the following link:

https://github.com/spectrecoin/spectre/releases/download/v1.4.0-alpha/Prebuild.Spectre.libraries.zip

Clone Wisp source. You can simply download a “Zip” from github.


Now unzip Prebuild Wisp libraries.zip that you just downloaded into the source root folder. Once done properly you should end up with “src”, “packages64bit” and “tor” all into one folder. Here is a screenshot of how it looks like after all the files are living together in the same folder.

![alt text](https://github.com/spectrecoin/spectre/raw/master/doc/Folder%20stucture.png)

Now go ahead and open a the file src/src.pro (It should open up with Qt Creator). Make sure our MSVC 64 bit compiler is selected. Click configure and build and run as usual with Qt.

