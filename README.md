[![GitHub version](https://img.shields.io/github/release/MattFryer/Qlik-Notepad-plus-plus.svg)](https://github.com/MattFryer/Qlik-Notepad-plus-plus/releases/latest)
[![GitHub Release Date](https://img.shields.io/github/release-date/MattFryer/Qlik-Notepad-plus-plus.svg)](https://github.com/MattFryer/Qlik-Notepad-plus-plus/releases/latest)
[![GitHub download](https://img.shields.io/github/downloads/MattFryer/Qlik-Notepad-plus-plus/total.svg)](https://github.com/MattFryer/Qlik-Notepad-plus-plus/releases/latest)
[![GitHub stars](https://img.shields.io/github/stars/MattFryer/Qlik-Notepad-plus-plus.svg)](https://github.com/MattFryer/Qlik-Notepad-plus-plus/stargazers)
[![GitHub issues](https://img.shields.io/github/issues-raw/MattFryer/Qlik-Notepad-plus-plus.svg)](https://github.com/MattFryer/Qlik-Notepad-plus-plus/issues)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/MattFryer/Qlik-Notepad-plus-plus.svg)](http://isitmaintained.com/project/MattFryer/Qlik-Notepad-plus-plus "Average time to resolve an issue")
[![GitHub license](https://img.shields.io/github/license/MattFryer/Qlik-Notepad-plus-plus.svg)](https://github.com/MattFryer/Qlik-Notepad-plus-plus/blob/master/LICENSE)

# Qlik Language Definition for Notepad++

The Qlik Custom Language Definition for Notepad++ gives basic syntax highlighting, auto-completion and code tool-tips when working with QlikView and Qlik Sense script files in Notepad++.

The syntax highlighting that is provided is limited to the capabilities of Notepad++ Custom Language Definitions and Auto-Completion files, and is an approximation of what you would get in Qlik's Edit Script dialog. It currently supports the following features:

* Highlighting of all current (v11.20) functions 
* Highlighting of all current (v11.20) keywords and statements 
* Highlighting of line comments (//) and block comments (/* */) 
* Folding of comments and code blocks including IF, SWITCH, FOR, DO and SUB statements 
* Auto-completion of all current functions, keywords and statements 
* Code tool tips for most commonly used functions
* Subroutines, qualify and unqaulify statements, table loads, info loads, mapping loads and store statements all identified within the function list.

If you find any keywords or functions missing then please let me know by reporting an issue and I'll add them to the next release. Support may also be added for subroutines within Qlik code libraries. If you'd like me to add support for your library, again please contact me.


## Installation
Here are the steps to get it installed and working yourself:

1. If you don't already have it, you can download Notepad++ from http://notepad-plus-plus.org/download/. Its completely free and a great text editor. If you are running an older version of Notepad++ then you will need to upgrade to the latest version in order to ensure the language definition will work correctly. Note: this latest release will definitely not work with versions of Notepad++ prior to v6.4.1
2. Download the Qlik language definition latest release ZIP archive file from https://github.com/MattFryer/QlikView-Notepad-plus-plus/releases/latest
3. Unpack the 3 XML files from the archive to a folder on you hard drive. 
4. Copy the "qlikview.xml" file from the folder to "%ProgramFiles(x86)%\Notepad++\plugins\APIs\". Tip: you can copy the path (including the % part) into Windows Explorer address bar. Windows may ask you to provide administrator privileges. 
5. Copy the "functionList.xml" file from the folder to "%UserProfile%\AppData\Roaming\Notepad++\". Tip: you can copy the path (including the % part) into Windows Explorer address bar. Windows may ask you to provide administrator privileges. If prompted to overwrite an existing version of the file, do so. 
6. Open Notepad++ and navigate the menu to Language -> Define your language...
7. Either a floating window or a panel to the right will appear, click on the "Import..." button within it.
8. Navigate to the folder where you saved the XML files and select the "qlikview-lang-def.xml" file before clicking "OK".
9. Hide the language panel by again selecting Language -> Define your language... on the menu. 


## Upgrade
If you already have a previous version of the Qlik language definition installed you will need to follow these steps to remove it and install the latest version:

1. This latest release supports new features found in the language definitions for Notepad++ version 6.4.1 and greater, If you are running a previous version you will need to upgrade Notepad++ before continuing further. You can download the latest version from http://notepad-plus-plus.org/download/.
2. Download the Qlik language definition latest release ZIP archive file from https://github.com/MattFryer/QlikView-Notepad-plus-plus/releases/latest
3. Unpack the 3 XML files from the archive to a folder on you hard drive. 
4. Copy the "qlikview.xml" file from the folder to "%ProgramFiles(x86)%\Notepad++\plugins\APIs\". Tip: you can copy the path (including the % part) into Windows Explorer address bar. Windows may ask you to provide administrator privileges. If prompted to overwrite an existing version of the file, do so.
5. Copy the "functionList.xml" file from the folder to "%UserProfile%\AppData\Roaming\Notepad++\". Tip: you can copy the path (including the % part) into Windows Explorer address bar. Windows may ask you to provide administrator privileges. If prompted to overwrite an existing version of the file, do so.
6. Open Notepad++ and navigate the menu to Language -> Define your language...
7. Either a floating window or a panel to the right will appear. Under the User Language drop down, select "QlikView" and then click the "Remove" button.
8. When asked to confirm if you wish to remove the current language, select "Yes".
9. Now, click on the "Import..." button.
10. Navigate to the folder where you saved the XML files and select the "qlikview-lang-def.xml" file before clicking "OK".
11. Hide the language panel by again selecting Language -> Define your language... on the menu.


## How To Use
If you open a .qvs file, Notepad++ will automatically identify it as a Qlik script file and apply the language definition for you. If you are creating a new file or using a different file extension then you'll need to change the language using the menu Language -> Qlik.

When typing, Notepad++ will suggest keywords and function to complete what you started to type. When you type a function name followed by the opening bracket (, where possible Notepad++ will display a tool tip showing a description of the function and the correct syntax.

To view the function list panel, select View -> Function List from the menu bar. The function list will identify many statements within the Qlik script file.

To enable auto-completion, select Settings -> Preferences... from the menu bar. Select Auto-Completion from the list on the left and then ensure the options are set as follows:

The options under Auto-Insert are optional and enable auto insertion of closing brackets and quotes are automatically entered when an opening bracket or quote is typed.


Disclaimer
===============================================
This language definition is provided free of charge, as is, with no warranties or guarantees. Neither Datoniq Limited or QlikViewAddict.com (including any of it's contributors) accept any liability for problems or loss resulting from it's use. Qlik is a registered trademark of QlikTech International AB.
