# This is a workaround to use global shortcuts for TODOIST on WINDOWS 10 (V2.0.0)

<br>

Since TODOIST its Windows 10 app doesn’t support global shortcuts at the moment. I made 2 little workarounds for the "open TODOIST" global shortcut.

    1. AutoHotKey workaround (Easy to set up, fast and Reliable)
    2. Vbs Workaround (Hard to setup, can be slow)
	
These workarounds add the following global TODOIST shortcuts to WIN 10:

    - alt+ctrl+a (Add new task)
    - alt+ctrl+s (open todoist)

:warning: **NOTE:** This is a mirrored repository the original repository can be found on [github](https://github.com/rickstaa/Todoist_Global_Shortcuts_WIN10).:warning:

## INSTRUCTIONS AutoHotKey workaround
1. [Download AutoHotKey.](https://autohotkey.com/)
2. Install AutoHotKey.
3. [Download the Workaround.](https://github.com/rickstaa/Todoist_Global_Shortcuts_WIN10/archive/master.zip)    	
4. Unzip the Workaround file.
5. Go to the "Todoist_Global_Shortcuts_WIN10\TODOIST_AHK" folder.
6. Click on the `installer.vbs` or `installer_todoist_preview.vbs` file to install the workaround.
    - Use the `installer.vbs` file to install the global shortcut for the regular "Todoist" windows 10 app.
    - Use the `installer_todoist_preview.vbs` file to install the global shortcut for the "Todoist Preview" windows 10 app.

## FAQ 

### The workaround is not working what now?
- Make sure AutoHotkey is running on startup.
- Ensure that you have the right user privileges to add files to your user startup folder.
- Still not working go to https://github.com/rickstaa/Todoist_Global_Shortcuts_WIN10/issues

### How does this workaround work?
A windows 10 universal app can be loaded by using its AppUserModelIDs. This is done by running the following command:

	explorer shell:AppsFolder/AppUserModelID

In this command the "AppUserModelID" refers to the AppUserModelID of the app you want to load. An excellent guide on how to find the AppUserModelID is located on:

- https://jcutrer.com/howto/windows/find-aumid

When the AppUserModelID is found, it can be used in to create an "AutoHotKey" file. This workaround just automates this process.

### What is the VBS workaround?
This workaround is the first workaround I created it can be used by people that don't like using AutoHotKey. See the README.txt in the TODOIST_VBS folder for instructions.
