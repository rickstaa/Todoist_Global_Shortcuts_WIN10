## This is a workaround to use global shortcuts for TODOIST on WINDOWS 10
_Created on 05/07/2017 - Version 2.0_

Since TODOIST its Windows 10 app doesn’t support global shortcuts at the moment. I made a  little workarounds for the "open TODOIST" global shortcut.

    - alt+ctrl+a (Add new task)
    - alt+ctrl+s (open todoist)

### Instructions AutoHotKey workaround
1. [Download AutoHotKey.](https://autohotkey.com/)
2. Install AutoHotKey.
3. [Download the Workaround.](http://github.com/rickstaa/Todoist_Global_Shortcuts_WIN10/archive/master.zip)
4. Unzip the Workaround file.
5. Go to the "Todoist_Global_Shortcuts_WIN10\TODOIST_AHK" folder.
6. Click on the "installer.vbs" file to install the workaround.

## FAQ

### The download link is not working for me what now?
If the download link fails for some reason try the "zip file download button" in the left right corner. If that also fails go to the project repository by clicking on the "View on github button". On this repository page click the "Clone/Download" button and then the "Zip" button.
![download button](https://github.com/rickstaa/Todoist_Global_Shortcuts_WIN10/blob/gh-pages/images/download_button.png)


### The workaround is not working what now?
- Make sure AutoHotkey is running on startup.
- Ensure that you have the right user privileges to add files to your user startup folder.
- Still not working go to [https://github.com/rickstaa/Todoist_Global_Shortcuts_WIN10/issues](https://github.com/rickstaa/Todoist_Global_Shortcuts_WIN10/issues)

### How does this workaround work?
A windows 10 universal app can be loaded by using its AppUserModelIDs. This is done by running the following command:

	explorer shell:AppsFolder/AppUserModelID

In this command the "AppUserModelID" refers to the AppUserModelID of the app you want to load. An excellent guide on how to find the AppUserModelID is located on:

- [https://jcutrer.com/howto/windows/find-aumid](https://jcutrer.com/howto/windows/find-aumid)

When the AppUserModelID is found, it can be used in to create an "AutoHotKey" file. This workaround just automates this process.

### What is the VBS workaround?
This workaround is the first workaround I created it can be used by people that don't like using AutoHotKey. See the README.txt in the TODOIST_VBS folder for instructions.
