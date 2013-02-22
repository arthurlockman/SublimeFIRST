SublimeFIRST
=========
A system for building FIRST Robotics C++ projects with Sublime Text. Finally, you can break free from WindRiver.

Prerequisites
---
In order for this build system to run, you have to install and configure [UCPP](https://github.com/nikitakit/ucpp), and ensure that you can build a project with it. This will require that you install Wine and wput if you're on a Mac or Linux machine. The easiest way that I found to configure it is to use the linux-windriver variant, and have an existing WindRiver install to go off of. 

Make sure that you create a symbolic link to the ucpp/ucpp folder in your bin. Do this by running this command (edit out the part that says "PATH_TO_UCPP" and replace it with the path to your UCPP base install.

	cd /opt/local/bin
	ln -s /[PATH_TO_UCPP]/ucpp/ucpp 

Instructions
---
Install the FRC.sublime-build script into your **~/[Sublime Text Settings Folder]/Packages/User** folder by just dropping it in (on the Mac, this folder is in ~/Library/Application Support/Sublime Text 2/Packages/User). You should then be able to select FRC from your Tools > Build System menu. 

If you've never built your project with UCPP before, you'll need to follow these next instructions. Once you've selected FRC as a build system, bring up the ST command prompt by pressing **Command-Shift-P**. Type "UCPP Setup" into that box. Press enter, and wait for it to finish. Then, bring up the same prompt and type "UCPP Regenerate Makefile". Once that's done, you should be able to just press **Command-B** to build your project, and **Command-Shift-B** to upload it.

Usage
---
Simply press **Command-B** to build the project using UCPP. Build errors will show up in the ST 2 console. 

Press **Command-Shift-B** to build and upload the project to the robot. 

Press **Command-Shift-P** and type in **UCPP Regenerate Makefile** every time you add or remove files from the project to regenerate the project's makefile. 

Notes
---
Anyone can use this code to build their projects. I can't guarantee it'll work for everyone, but I can try to help if it doesn't. Please also note that this build system isn't complete yet. I'm still adding features. It will be complete by the time the 2013 season rolls around, so that it can be used for actual development. 

Please post issues if they are found. I'll fix anything that is posted.
