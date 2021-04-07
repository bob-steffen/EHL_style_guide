# EHL CODING STYLE GUIDE/BEST PRACTICES

## 1 Background

This document exists to increase the efficiency and productivity of both programmers (people who write code) and users (people who use code as tools for other tasks)
by defining clear and easy to follow guidlines for writing and maintaining code.

Without futher ado, the EHL style guide.

## 2 Code Editors

VSCode is the defacto code editor because it is easiest to configure, and has access to superior langauge servers for linting made by Microsoft.

### 2.1 VSCode

#### 2.1.1 Installation

For computers running Windows, Mac or Linux VSCode can be installed here: <https://code.visualstudio.com/download>

For RaspberryPis run these commands in the terminal:

    sudo apt update

    sudo apt install code

and VSCode will appear under the progamming tab:

![alt text](running_vs_code_on_rasp_pi.png "Running VSCode on a Raspberry Pi")

reference: <https://code.visualstudio.com/docs/setup/raspberry-pi>

#### 2.1.2 Configuration

##### 2.1.2.1 Extensions

In VSCode you will find a button that looks like this where you can install extensions.

![alt text](extensions_icon.png "VSCode Extensions Icon")

By default VSCode provides IntelliSense (suggestions on how to improve and/or bugfix code as you write it) only for Javascript, but this functionality is available for all other major languages as extensions.

Depending on the language you wish to program in, you should go to the extensions tab in VSCode and search for the name of that langauge. If there is an extension made by Microsoft, download that one. Otherwise, choose whichever is most popular.

![alt text](language_server_search.png "Searching for language support in VSCode")

Here a few recommended extensions to get you started (open a terminal in vs code and then paste these in and hit enter):

    code --install-extension aaron-bond.better-comments
    code --install-extension CoenraadS.bracket-pair-colorizer-2
    code --install-extension eamodio.gitlens
    code --install-extension Gruntfuggly.todo-tree
    code --install-extension mihelcic.colored-regions
    code --install-extension ms-python.python
    code --install-extension ms-python.vscode-pylance
    code --install-extension ms-vscode-remote.remote-containers
    code --install-extension ms-vscode-remote.remote-ssh
    code --install-extension ms-vscode-remote.remote-ssh-edit
    code --install-extension ms-vsliveshare.vsliveshare
    code --install-extension ms-vsliveshare.vsliveshare-pack
    code --install-extension njpwerner.autodocstring
    code --install-extension PKief.material-icon-theme
    code --install-extension Tyriar.terminal-tabs
    code --install-extension uctakeoff.vscode-counter
    code --install-extension wayou.vscode-todo-highlight
    code --install-extension zhuangtongfa.material-theme

##### 2.1.2.2 Python Specific Settings

Although Python allows for dynamic types, it is best practice to define variable types using the python `typing` library. You can do this by adding `from typing import <insert primitive datatype name here>` or just `from typing import *` if you're lazy.

VSCode will enforce these types by indicating that there are errors in your script only if you enable it in the Pylance Extension's settings.

To do so, click the settings button in the bottom left hand corner of the screen while in VSCode.

![alt text](settings_icon.png "VSCode Settings Icon")

then click `Settings`

![alt text](click_settings_button.jpg "Click the Settings option!")

then click on `Extensions`

![alt text](click_extensions_button.jpg.png "Click the Extensions option!")

then click on `Pylance`

![alt text](click_pylance_button.jpg.png "Click the Pylance option!")

then scroll around and find the `Type Checking Mode` setting and set it to `basic`:

![alt text](change_type_checking_setting.jpg "Change the 'Type Checking Mode' setting to 'basic'!")

You're all set!

## 3 Coding Styles and Standards

It is critical to the EHL team that a standard is followed for coding so that code can be easily understood and reused. As the EHL continues to innovate and grow new languages will be introduced and new cases that are not explicitly covered in this guide will arise. In either event it is imperative that this style guide is updated to explain what to do and how to do it.

### 3.1 Python

For Python styling, reference: <https://google.github.io/styleguide/pyguide>

This is the standard by which all python code should be written.

A more condensed version of this document that is specific to EHL will come soon.

### 3.1 C++

Follow the guidelines as taught in the CS 142/235 courses @ BYU.

A summary of these will be provided soon.