SublimeFIRST
=========
A system for building FIRST Robotics C++ projects with Sublime Text. Finally, you can break free from WindRiver.

Prerequisites
---
In order for this build system to run, you have to install and configure [UCPP](https://github.com/nikitakit/ucpp), and ensure that you can build a project with it. This will require that you install Wine and wput if you're on a Mac or Linux machine. The easiest way that I found to configure it is to use the linux-windriver variant, and have an existing WindRiver install to go off of. 

Instructions
---
Configure the project which you want to build with SublimeFIRST using **ucpp configure** and **ucpp init**. Then, install the FRC.sublime-build script into your **~/[Sublime Text Settings Folder]/Packages/User** folder by just dropping it in (on the Mac, this folder is in ~/Application Support/Sublime Text 2/Packages/User). You should then be able to select FRC from your Tools > Build System menu. 

Usage
---
Simply press **Command-B** to build the project using UCPP. Build errors will show up in the ST 2 console. 

Press **Command-Shift-B** to upload the project to the robot. Remember to press Cmd-B first, to ensure that you are uploading the most recent compile of the code.

Notes
---
Anyone can use this code to build their projects. I can't guarantee it'll work for everyone, but I can try to help if it doesn't. Please also note that this build system isn't complete yet. I'm still adding features. It will be complete by the time the 2013 season rolls around, so that it can be used for actual development. 

Please post issues if they are found. I'll fix anything that is posted.