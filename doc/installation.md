# Installation

```{todo}
This information is not part of the Plover Wiki or Read the Docs documentation. While steps have been taken to ensure accuracy, follow these instructions at your own discretion.
```

## From Binaries

### System requirements

- Plover requires about 250 MB minimum free space. More space is required if you install additional plugins, add more dictionaries, or install required dependencies.
- Using keyboard customizers like text expanders or [text replacements](https://support.apple.com/guide/mac-help/mh35735/mac) may cause unintended behavior when writing with Plover.
- Requires an Internet connection to download and install plugins.

**Windows**

- Intel or AMD processor.
- Administrator account required to use a stenography (steno) keyboard requiring hardware drivers to be installed separately.

**macOS**

- Apple silicon or Intel processor.
- macOS Monterey 12.0 or later.
- Administrator account required to allow Plover to use accessibility features.

**Linux**

- Intel or AMD processor.
- X11 or Wayland-based desktop environment. Plover may behave unexpectedly in certain applications with Wayland-based desktop environments (like GNOME included in Ubuntu and Fedora).
- Desktop environment with a system tray so that Plover’s menu item can be accessed.
- GNOME may require additional extensions to enable system tray features.
- Administrator account required to install device specific (udev) rules, and dependencies. If you want to use a steno keyboard, additional system configuration is required.

### Download Plover

Visit Plover’s [latest release](https://github.com/openstenoproject/plover/releases/latest) page. Expand Assets, then choose one of the following to download Plover:

- If you’re using Windows: Choose “Windows: Installer,” or “Windows: Portable ZIP.”
- If you’re using macOS: **Choose “macOS: Disk Image.”
- If you’re using Linux: Choose “Linux: AppImage.”

If you need to download a pre-release or older version of Plover, see Plover’s [release](https://github.com/openstenoproject/plover/releases/) page.

### Install Plover for Windows

Because Plover hasn’t been digitally signed, you may see messages appear about Plover from an unknown publisher or that it isn’t commonly downloaded. Make sure to only download Plover from Open Steno Project on GitHub: https://github.com/openstenoproject/plover/releases.

#### What’s the difference between the Installer and Portable ZIP?

- *Installer:* Plover will be installed for all users on your computer. However, your settings are paired to your own user account. For example, your preferred dictionaries and installed plugins will only apply for you. When you’re not logged on, other users can open Plover but their settings will be different.
- *Portable ZIP:* The Portable ZIP provides flexibility when using Plover on different computers and lets you keep multiple copies of Plover with different settings. For example, when you use a shared computer at a public location — such as a school or library that allow opening applications from other sources, you can open Plover from external devices, such as USB drives.

#### Use the Installer

1. When a “plover-[version]-win64.exe isn’t commonly downloaded” message appears in the Downloads menu, click the ellipsis (…) next to the file’s name, then choose Keep.
2. Below the “Make sure you trust plover-[version]-win64.exe before you open it” message, select the ellipsis, then choose Keep anyway.
3. Open plover-[version]-win64.exe. For example, plover-5.1.0-win64.exe.
4. If a “Windows protected your PC” message appears, click More info, then choose Run anyway.
5. If a User Account Control message appears, choose Yes and follow the onscreen instructions.

If you created Plover Start menu shortcuts: To open Plover, select the Start menu, type “plover,” then choose “Plover [version]”.

#### Use the Portable ZIP

1. If a “Make sure you trust plover-[version]-win64.zip before you open it” message appears, click Show more, then choose Keep anyway.
2. Right-click plover-[version]-win64.zip, then choose “Show in folder” from the shortcut menu. For example, plover-5.1.0-win64.zip. 
    
    The zip file appears in a File Explorer window. 
    
3. Right-click plover-[version]-win64.zip, then choose Extract All from the shortcut menu.
4. In the “Extract Compressed (Zipped) Folders” window, choose a folder to store Plover portable in, then choose Extract.
    
    If “Show extracted files when complete” is unselected, you will need to locate the Plover folder you extracted.
    
#### Enable Portable Mode

Portable Mode stores Plover’s settings in the same folder as the Plover app — keeping it separate from your Windows AppData folder and other versions of Plover.

1. Locate the Plover portable folder you extracted.
2. In the Plover portable folder window, turn on file name extensions:
    - *Windows 11:* Choose View > Show > File name extensions so that a tick appears next to the option.
        
        If you don’t see the View menu, select the ellipsis (…).
        
    - *Windows 10:* Choose View > File name extensions in the Show/hide section, if unselected.
        
        If you don’t see “File name extensions,” click Show/hide.
        
    
    Alternatively, you can turn on file name extensions using the File Explorer Options Control Panel:
    
    - Select the Start menu, type “File Explorer Options,” then press Enter.
        
        Select the View tab.
        
        Below Advanced settings, unselect “Hide extensions for known file types” if selected, then choose OK.
        
3. Right-click in the Plover portable folder, choose New > Text Document from the shortcut menu, then name the file “plover.cfg”.
4. Double-click plover.exe to open Plover. 
    
    If a “Windows protected your PC” message appears, click More info, then choose Run anyway.

Plover copies its included dictionaries into its portable folder.

### Install Plover for macOS
#### Check which macOS is installed

Steps in this guide are based on the version of macOS your Mac is using. Before you continue, [find out which macOS your Mac is using](https://support.apple.com/109033).

#### Use the Disk Image
1. Open plover-[version]-macosx_12_0_universal2.dmg. For example, plover-5.1.0-macosx_12_0_universal2.dmg. The Plover disk image appears in a Finder window.
    
    *Note:* Plover versions earlier than 5.0.0 are named plover-[version]-macosx_10_13_x86_64.dmg.
    
2. Drag the Plover icon into your Applications folder. 

After installation completes, choose File > Eject.
3. In the Finder, click Applications in the sidebar, Control-click the Plover app, then choose Open from the shortcut menu.

#### ~~Open the Plover main window~~
~~The Plover status menu icon only appears in macOS Sequoia or earlier.~~ 

~~To show Plover’s main window:~~

- *macOS Tahoe or earlier:* Click the Plover icon in the Dock then choose File > Show.
- *macOS Sequoia or earlier:* Click the Plover status menu item in the right end of the menu bar then choose Show.

#### If you can’t open or need to use an earlier version of Plover

Because certain versions of Plover for macOS hasn’t been digitally signed or notarized, you may see messages appear that it can’t be checked for malware or its developer is not verified. Make sure to only download Plover from Open Steno Project on GitHub: https://github.com/openstenoproject/plover/releases.

Follow these steps if you installed one of the following versions of Plover on a Mac that includes a specific [kind of processor](https://support.apple.com/116943):

- Apple silicon or Intel with Plover 5.0.0 or earlier.
- Intel with Plover 5.1.0 to 5.2.1 using Open Core Legacy Patcher.

Plover 5.1.0 introduces a bug that causes Plover to not respond on Intel Macs. macOS running using patching tools such as Open Core Legacy Patcher are not affected. This is fixed in Plover 5.2.2.

If you have a Mac with Apple silicon without [Rosetta](https://support.apple.com/102527) installed, you may be automatically asked to install it, because versions of Plover earlier than 5.0.0 were built for Intel-based Macs.

To authorize Plover to open:

**macOS Sequoia or later**

1. If you see a “’Plover’ Not Opened” message, choose Done. 
2. Open System Settings, click Privacy & Security, scroll down until you see the Security section. 
3. Click Open Anyway on the right of the “’Plover’ was blocked to protect your Mac” message. 
4. A message asking you to open Plover appears, choose Open Anyway. If prompted, enter your details.

**macOS Sonoma**

1. If you see a “’’Plover’ can’t be opened because Apple cannot check it for malicious software” message, choose OK.
2. Open System Settings, click Privacy & Security, scroll down until you see the Security section.
3. Click Open Anyway below the “’Plover’ was blocked from use because it is not from an identified developer” message. 
4. A message asking you to open Plover appears, choose Open Anyway. If prompted, enter your details.

**macOS Ventura or earlier** 

If you see a “macOS cannot verify the developer of ‘Plover’. Are you sure you want to open it?” message, choose Open.

#### Allow Plover to control your Mac

When Plover has its output enabled and accessibility permissions turned on, you will be able to interact within applications using Plover.

**Why does Plover need to control my computer?**

Plover interacts within applications outside of Plover by checking your machine’s input — such as a computer or steno keyboard for any keys that have been pressed. When these key combinations match definitions, known as translations in Plover’s dictionaries, Plover is responsible for typing keystrokes that form the translation in the application you’re using. These translations may include words, numbers, or keyboard shortcuts.

#### If you have updated, reinstalled or moved Plover

You must make changes to the list of accessibility permissions (even if it looks like Plover has been granted permission), then do one of the following:

- Turn off then turn on Plover’s accessibility permission.
- Remove Plover from the list of accessibility permissions then add it to the list.

If changes don’t appear to take effect, you may need to restart your Mac before you can write using Plover.

#### **If a “’Plover’ would like to control this computer using accessibility features” message appears**

**macOS Ventura or later**

1. Choose Open System Settings. 
    
    The Privacy & Security settings’ Accessibility section appears.
    
2. Turn on the accessibility permission to the right of the Plover app in the list.
3. If prompted, enter an administrator account’s details.
4. Quit Plover, then open it again for changes to take effect.

**macOS Mojave and earlier**

1. Choose Open System Preferences. 
    
    The Security & Privacy settings appears.
    
2. Click Accessibility on the left, then select Plover’s tick box.
    
    If you can’t allow Plover to control your computer, click the lock, then enter an administrator account’s details.
    
3. Quit Plover, then open it again for changes to take effect.

#### **Check accessibility permissions**
If you want to check if Plover has been granted accessibility permission or need to change Plover’s permission, you can review the list of accessibility permissions.

**macOS Ventura or later**

1. Open System Settings, click Privacy & Security, click Accessibility in the sidebar, then click Accessibility on the right.
2. Do any of the following:
    - *Add Plover to the list:* Click the add (+) button at the bottom of the list, locate the Plover app, select the Plover app, then click Open.
    - *Grant Plover permission:* Select Plover’s tick box on the right.
    - *Deny Plover permission:* Unselect Plover’s tick box on the right.
    - *Remove Plover from the list:* Select Plover, then click the remove (−) button at the bottom of the list.
3. Quit Plover, then open it again for changes to take effect.

**macOS Monterey and earlier**

1. Open System Preferences, click Security & Privacy, then click Accessibility on the left. 
2. Do any of the following:
    - *Add Plover to the list:* Click the add (+) button at the bottom of the list, locate the Plover app, select the Plover app, then click Open.
    - *Grant Plover permission:* Select Plover’s tick box.
    - *Deny Plover permission:* Unselect Plover’s tick box.
    - *Remove Plover from the list:* Select Plover, then click the remove (−) button at the bottom of the list.
3. Quit Plover, then open it again for changes to take effect.

### Install Plover for Linux

These sections are based on Ubuntu and Fedora using the GNOME Desktop Environment. Menu items and options may appear different in other desktop environments and Linux distributions.

Plover works best when using a X11-based desktop environment. Plover also works with Wayland-based desktop environments (like GNOME included in Ubuntu and Fedora). However, it may behave unexpectedly in certain situations.

#### Use the AppImage

After you download Plover, you’ll need to make the Plover AppImage executable before you can open it.

1. In the Files app, locate the folder with Plover’s Appimage then do one the following to open a console window:
    - *Ubuntu:* Right-click an empty space within the folder, then choose Open in Terminal from the shortcut menu.
    - *Fedora:* Right-click an empty space within the folder, then choose Open in Console from the shortcut menu.
    
    On a default installation of Ubuntu and Fedora, the console window appears using an app called Terminal.
    
2. In the console window, make Plover executable using the following command, replacing *plover.AppImage* with the name of the Plover AppImage you downloaded previously. Then press Enter.
    
    `chmod +x ./plover.AppImage` 
    
    *Example:* *chmod +x ./plover-4.0.3-x86_64.AppImage*
    
3. Type the following command, then press Enter to verify if Plover can start correctly:
    
    `./plover.AppImage` 
    
    *Example:* *./plover-4.0.3-x86_64.AppImage* 
    
    Wait a few seconds. If Plover appears, skip to Step 5.
    
4. The console window displays error information about the AppImage being opened. If a “AppImages requires FUSE to run” message appears in the console window, do one of the following:
    - *Install FUSE on Ubuntu 24.04 or later:* Type or paste `sudo apt install libfuse2t64` in the console window then press Enter. After installation completes, open the Plover AppImage file.
    - *Install FUSE on Fedora:* Type or paste `sudo dnf install fuse fuse-libs` in the console window then press Enter.  After installation completes, open the Plover AppImage file.
    - *Extract the AppImage file:* Type the following command in the console window, then press Enter.
        
        `./plover.AppImage --appimage-extract`
        
        Example: *./plover-4.0.3-x86_64.AppImage --appimage-extract*
        
        The extracted contents of the AppImage appears in a folder named squashfs-root (you may want to rename this folder).
        
        Open the extracted AppImage, right-click AppRun, then choose Run as a Program from the shortcut menu.
        
    - *Install FUSE on other distributions:* See [https://github.com/AppImage/AppImageKit/wiki/FUSE](https://github.com/AppImage/AppImageKit/wiki/FUSE).
    
    It’s recommended that you install FUSE so you don’t need to extract the AppImage when updating to a later version of Plover.
    
5. If a message about requiring authentication or installing udev rules appears, enter your details, then press Enter.
6. Restart your computer for changes to take effect.

You can double-click the AppImage to open Plover instead of using a console window to open Plover. 

After you open Plover, it appears as org.openstenoproject.python in the task manager, if available.

#### Unexpected no authorization protocol error

If you see a message about no authorization protocol (it may be too long to display on the screen), you’re using a Wayland-based desktop environment. You need to grant permission for your user to use the X Server.

#### Temporarily grant permission to the X Server

1. In a console window, type or paste `xhost +si:localuser:$USER` , then press Enter.
2. Open Plover.

When you log out or restart your computer, you’ll need to repeat these steps before you can open Plover.

#### Automatically grant permission to the X Server using a shell script and app shortcut

To automatically grant your user X Server permission when you open Plover, use a shell script, and app shortcut—also known as a desktop entry file to automatically run the script when you run the app shortcut.

1. If needed, move the Plover AppImage to a new location.
2. Create a new shell script (.sh) file with the following content, replacing */location/Plover-[version]-x86_64.AppImage* with the path to the Plover AppImage.

```
#!/bin/bash
xhost +si:localuser:$USER
/location/Plover-[version]-x86_64.AppImage
```

Example: *$HOME/Documents/Plover/plover-4.0.3-x86_64.AppImage*

1. Make the shell script executable. Open a console window, type the following command, replacing */location/plover-wayland.sh* with the path to the shell script. Then press Enter.

`chmod +x */location/plover-wayland.sh*`

*Example: chmod +x $HOME/Documents/Plover/plover-wayland.sh.*
2. Create a new app shortcut (.desktop) file with the following content, replacing */location/plover-wayland.sh* with the path to the shell script.

```
[Desktop Entry]
Type=Application
Terminal=false
Exec=/location/plover-wayland.sh
Name=Plover
Icon=/location/plover-icon.svg
Categories=Utility;Accessibility;
Comment=Stenographic Input Tool
Keywords=steno;input;keyboard;
X-Unity-IconBackgroundColor=#414F4C
```

Example: *Exec=$HOME/Documents/Plover/plover-wayland.sh*

1. If you don’t want an icon to appear on the app shortcut, delete the `Icon=` line. Then skip to Step 7.
2. If you want the Plover icon to appear on the app shortcut, save the [Plover icon](https://raw.githubusercontent.com/openstenoproject/plover/main/plover/assets/plover-icon.svg) to a folder. Then replace */location/plover-icon.svg* with the path to the icon.
    
    *Example: $HOME/Documents/Plover/plover-icon.svg*
    
3. Save the app shortcut file with the .desktop file extension.
    
    *Example: plover.desktop.*
    
4. Double-click on it to open Plover.

#### Qt Platform plugins and xcb error

You’ll need to install additional dependencies before Plover can be opened in Wayland-based desktop environments.

#### Dependencies

If you aren’t using a Linux distribution based on Ubuntu or Fedora, make sure that the following packages are installed:

- qt5-style-plugins
- libxcb-cursor0
- libxcb
- libxcb-utill

These package names may be slightly different in some package repositories. For example, libxcb is packaged as libxcb1 on Ubuntu.

#### Install qt5-style-plugins

Install qt5-style-plugins by doing the following:

1. Open a console window. 
2. Type or paste one of the following commands then press Enter:
    - *Ubuntu:*  `sudo apt install qt5-style-plugins`
    - *Fedora:* `sudo dnf install qt5-qtstyleplugins`
3. If prompted, type your details then press Enter. 
4. Type Y, then press Enter.

#### Install libxcb-cursor (Wayland)

The X protocol C-language Binding (XCB) cursor platform library enables Plover to write text into X11-based applications.

Install libxcb-cursor0 by doing the following:

1. Open a console window.
2. Type or paste one of the following commands then press Enter:
    - *Ubuntu:* `sudo apt install libxcb-cursor0`
    - *Fedora:* `sudo dnf install libxcb`
3. If prompted, type your details then press Enter. 
4. Type Y, then press Enter.

*Note:* You don’t need to manually install libxcb1 or libxcb-util1 because both are automatically installed as libxcb-cursor0’s dependencies.

#### If you see an error about creating a new QApplication instance

> Please destroy the QApplication singleton before creating a new QApplication instance.
> 

The Plover app relies on the Qt Development framework and creates a session known as a QApplication instance that is responsible for Plover working with your desktop environment. 

The rest of this section is intentionally left blank.

#### GNOME Top Bar Item

The GNOME Desktop Environment, included with many Linux distributions (like Ubuntu and Fedora) requires extensions so that Plover’s menu item appears in GNOME’s top bar—also known as the top panel. 

If the Plover menu item doesn’t appear in the top of the screen (it looks like a steno key or a shield and may have a pause ⏸ or cross ❎ symbol), follow these steps.

1. From a web browser, go to the [GNOME Shell Extensions](https://extensions.gnome.org/) page (extensions.gnome.org).
2. If you see a message about installing GNOME Shell integration, follow the on-screen instructions to install the browser extension, then reload the page. 
3. If you see a “No such native application org.gnome.chrome_gnome_shell” message, open a console window, type or paste one of the following commands, then press Enter. 
    - *Ubuntu*: `sudo apt install gnome-browser-connector`
    - *Fedora:*  `sudo dnf install gnome-browser-connector`
    
    If prompted, enter your details, then press Enter.
    
    Type Y, then press Enter.
    
    After installation completes, reload the GNOME Shell Extensions page.
    
    For more information and installation instructions for other distributions, see: [GNOME browser integration - Installation guide](https://gnome.pages.gitlab.gnome.org/gnome-browser-integration/pages/installation-guide.html)
    
4. Do one of the following:
    - If a message asking you to start the WebExtension backend appears, choose Allow.
    - If you don’t see any messages above the “Search for extensions” field, skip to step 7.
5. Quit the web browser, and then open it.
6. Go to the [GNOME Shell Extensions](https://extensions.gnome.org/) page.
7. In the “Search for extensions” field, type “AppIndicator and KStatusNotifierItem”, then select “AppIndicator and KStatusNotifierItem Support” by 3v1n0.
    
    Alternatively, you can look for any other extension that restores tray icons to the top bar.
    
8. Turn on the extension on the right.
    
    If a message asking you to install the extension appears, choose Install.
    
The Plover menu item appears in the top of the screen.


## From Source

```{todo}
Complete this section.
```
