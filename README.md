Sublime Text - AppendSemicolonCommand
========================================

This is a simple plugin for Sublime Text 2 that will add a semicolon to the end of the current line without moving the cursor. This is really handy when working in a language, such as JavaScript, that makes use of semicolons. I am not the author, I found it in an [answer by 'skuroda' on Stack Overflow](http://stackoverflow.com/a/16954135/659501). I changed the name of it to something a little more descriptive of it's actual function.

I make use of it and wanted to make it easier for myself to install so I added it here. I would like to see the [answer's author](http://stackoverflow.com/users/1852931/skuroda) add it to the Package Control repository, but until then, I have it here so it is easier to install.

Usage
=====

Once installed, you will be able to press `command + ;` (Mac) or `ctrl + ;` (Windows/Linux) from anywhere within the line and a semicolon will magically appear at the end of the line.

Installation
============

Sublime Text 2 & 3 users
------------------------
Open up a terminal (command prompt for Windows people) and change directories into your Sublime Text Packages directory. If you aren't sure where this is located on your system, in Sublime, go to **Preferences** -> **Browse Packages** to find out. For Mac OS X users this will be either `~/Library/Application Support/Sublime Text 2/Packages` or `~/Library/Application Support/Sublime Text 3/Packages` depending on your installed version.

```bash
git clone https://github.com/dgarlitt/AppendSemicolonCommand.git
```

Sublime Text 2 users, you're not done yet
-----------------------------------------
checkout the ST2 branch to get the Sublime Text 2 version of the code

```bash
cd AppendSemicolonCommand
git checkout ST2
```

Key Binding
-----------
Add the following to your key binding preferences (**Preferences** -> **Key Bindings - User**):

```javascript
{ "keys": ["super+;"], "command": "append_semicolon" }
```
