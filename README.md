# Compiler-UPX-SIGN-TOOL-for-EXE-and-MSO-VBA
Special UPX &amp; SIGN TOOL for EXE and MSO-VBA
Hello Again!

I have created a QM-Progrämmli ähh Tool to Compress and or Sign my Proggis, DLL's or suitable MS-OFFICE Files...

You can use it with Quick Macros (QM-) Compiler or other Compiler (PureBasic etc.) or as a Standalone (Drag&Drop-) TOOL...

You need this:
The Wonderfull (now free) Automation Program:
Quick Macros - automation software for Windows. Some features:
Macro commands, including user interface automation, launching programs, file management, text processing (Autotext - Inserts text snippets using keyboard shortcuts) and custom dialogs.
Triggers, including hotkeys, mouse, scheduler, toolbars and menus.
Records keyboard and mouse actions.
Programming language with functions, classes, full API support.
You can create programs for various purposes, and run them in Quick Macros or as exe files.
Quick Macros is no longer being developed or updated. It has been superseded by LibreAutomate C#.
You can still download the last QM version, 2.4.12.2. Date 2021-08-22. For Windows 7, 8, 8.1, 10, 11.
Now it's free. Registration code: XVZVTCLELEFXEFMETVVZPCXFNMCRCFDN-Now%20it%27s%20free

The unpacked upx.exe from upx-5.0.2-win32.zip - (UPX - X86 Win32 version it is good for all) and the original Microsoft SignTools.exe must be placed in the same folder as of  UPX / SIGN Tool  Runner (e.g. in Subfolder "Plugins") or in a Subfolder from them named "CERT"

And of course you also need a suitable (ev. self-created...) SIGN (*.pfx) file for code certification (i put them in the Subfolder ...\CERT)...

To activate the functions for EXE (after!) Compiling you must make first an Entry (for each exe file) in QM Menu under Run Make Exe:
In Section: Run functions when creating a exe, After - insert the name of the tool (without extension!!!)
eg. Run_UPX_SIGN                                  (or rename Run_UPX_SIGN.exe to shorter e.g. MyUPX.exe) to have a smaller entry (only: MyUPX)

To sign MSO vba files too - you need
Microsoft Office Subject Interface Packages for Digitally Signing VBA Projects
See too: https://github.com/Joflixen/signtool and the headers of my QML source file...
Download the Windows SDK, and install the Code Signing component.
Once installed go to the install path, on my local workstation it was here: 
 C:\Program Files (x86)\Windows Kits\10\bin\10.0.19041.0\x86  (ONLY 32 BIT COMPONENT WORKS!!!)
Copy the x86 version of SignTool.exe to your working path... 
Download and run the Microsoft Office Subject Interface Package, during the installer it will ask for an installation path, choose a path like: 
Code:Copy      Help
C:\[workingpath]\MSOSIP
Refer to the readme.txt for additional instructions if required in "HOW TO USE THESE COMPONENTS

IMPORTANT: You must registered the two msosip*.dll Files with regsvr32.exe as Admin-User in a fixed directory and Place the vbe7.dll in them! (and you need ev. VC_redist.x86.exe...)

Call from cmd with run as Admin:
cd to the Install directory from msosip.dll... and run
C:\Windows\System32\regsvr32.exe msosip.dll and C:\Windows\System32\regsvr32.exe msosipx.dll

An informative RegSvr32 message box respectively should then appear...

wfg. from Schindi aus Austria

QML Source File can be Found in Link: https://www.libreautomate.com/forum/showthread.php?tid=7881 (= Thread:  Special UPX & SIGN TOOL for EXE and MSO-VBA)


