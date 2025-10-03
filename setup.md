---
title: Setup
---

## Download files

You need to download some files to follow this lesson.

1. Download [shell-lesson-data.zip][zip-file] and move the file to your Desktop.
2. Unzip/extract the file.
  **Let your instructor know if you need help with this step**.
  You should end up with a new folder called **`shell-lesson-data`** on your Desktop.

## Install software


:::::::::::::::::::::::::::::::::::::::::  callout

## Installation instructions {#instructions}

Follow these install instructions according to your Operating System (OS).


::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::: solution

### Windows {#windows1}

Please install **Git for Windows** using the instructions below.

- Download the Git for Windows <a href="https://gitforwindows.org/">installer</a>
installed.
- Run the installer and follow the steps below:
  - Click on "Next" four times (two times if you've previously installed Git).  You don't need to change anything in the Information, location, components, and start menu screens.
  - From the dropdown menu, "Choosing the default editor used by Git", select "Use the Nano editor by default" (NOTE: you will need to scroll <emph>up</emph> to find it) and click on "Next".
  - On the page that says "Adjusting the name of the initial branch in new repositories", ensure that "Let Git decide" is selected. This will ensure the highest level of compatibility for our lessons.
  - Ensure that "Git from the command line and also from 3rd-party software" is selected and click on "Next". (If you don't do this Git Bash will not work properly, requiring you to remove the Git Bash installation, re-run the installer and to select the "Git from the command line and also from 3rd-party software" option.)
  - Select "Use bundled OpenSSH".
  - Ensure that "Use the native Windows Secure Channel Library" is selected and click on "Next".
  - Ensure that "Checkout Windows-style, commit Unix-style line endings" is selected and click on "Next".
  - Ensure that "Use Windows' default console window" is selected and click on "Next".
  - Ensure that "Default (fast-forward or merge) is selected and click "Next"
  - Ensure that "Git Credential Manager" is selected and click on "Next".
  - Ensure that "Enable file system caching" is selected and click on "Next".
  - Click on "Install".
  - Click on "Finish" or "Next".
-  If your "HOME" environment variable is not set (or you don't know what this is):
  - Open command prompt (Open Start Menu then type <code>cmd</code> and press <kbd>Enter</kbd>)
  - Type the following line into the command prompt window exactly as shown: <p><code>setx HOME "%USERPROFILE%"</code></p>
  - Press <kbd>Enter</kbd>, you should see <code>SUCCESS: Specified value was saved.</code>
  - Quit command prompt by typing <code>exit</code> then pressing <kbd>Enter</kbd>

If you prefer, here is a video tutorial with the instructions: <a href="https://www.youtube.com/watch?v=339AEqk9c-8" target="_blank">https://www.youtube.com/watch?v=339AEqk9c-8</a>

::::::::::::

:::::::::::: solution

### MacOS {#macos1}

For a Mac computer running macOS Mojave or earlier releases, the default Unix Shell is Bash.
For a Mac computer running macOS Catalina or later releases, the default Unix Shell is Zsh.
Your default shell is available via the Terminal program within your Utilities folder.

To open Terminal, try one or both of the following:

- In Finder, select the Go menu, then select Utilities.
  Locate Terminal in the Utilities folder and open it.
- Use the Mac 'Spotlight' computer search function.
  Search for: `Terminal` and press <kbd>Return</kbd>.

To check if your machine is set up to use something other than Bash,
type `echo $SHELL` in your terminal window.

If your machine is set up to use something other than Bash,
you can run it by opening a terminal and typing `bash`.

[How to Use Terminal on a Mac][mac-terminal]

::::::::::::

:::::::::::: solution

### Linux {#linux1}

The default Unix Shell for Linux operating systems is usually Bash.
On most versions of Linux, it is accessible by running the
[Gnome Terminal][gnome-terminal] or [KDE Konsole][kde-konsole] or [xterm],
which can be found via the applications menu or the search bar.
If your machine is set up to use something other than Bash,
you can run it by opening a terminal and typing `bash`.

::::::::::::

## Open a new shell

After installing the software

3. Open a terminal.
  If you're not sure how to open a terminal on your operating system, see the instructions below.
4. In the terminal type `cd` then press the <kbd>Return</kbd> key.
  This step will make sure you start with your home folder as your working directory.

In the lesson, you will find out how to access the data files in this folder.

:::::::::::::::::::::::::::::::::::::::::  callout

## Where to type commands: How to open a new shell

The shell is a program that enables us to send commands to the computer and receive output.
It is also referred to as the terminal or command line.

Some computers include a default Unix Shell program.
The steps below describe some methods for identifying and opening
a Unix Shell program if you already have one installed.
There are also options for identifying and downloading a Unix Shell program,
a Linux/UNIX emulator, or a program to access a Unix Shell on a server.

If none of the options below address your circumstances,
try an online search for: Unix shell [your computer model] [your operating system].


::::::::::::::::::::::::::::::::::::::::::::::::::

:::::::::::: solution

### Windows {#windows2}

Computers with Windows operating systems do not automatically have a Unix Shell program
installed.
In this lesson, we encourage you to use an emulator included in [Git for Windows](#instructions),
which gives you access to both Bash shell commands and Git.

Once installed, you can open a terminal by running the program Git Bash from the Windows start
menu.

**For advanced users:**

As an alternative to Git for Windows you may wish to [Install the Windows Subsystem for Linux][wsl]
which gives access to a Bash shell command-line tool in Windows 10 and above.

Please note that commands in the Windows Subsystem for Linux (WSL) may differ slightly
from those shown in the lesson or presented in the workshop.

::::::::::::

:::::::::::: solution

### MacOS {#macos2}

For a Mac computer running macOS Mojave or earlier releases, the default Unix Shell is Bash.
For a Mac computer running macOS Catalina or later releases, the default Unix Shell is Zsh.
Your default shell is available via the Terminal program within your Utilities folder.

To open Terminal, try one or both of the following:

- In Finder, select the Go menu, then select Utilities.
  Locate Terminal in the Utilities folder and open it.
- Use the Mac 'Spotlight' computer search function.
  Search for: `Terminal` and press <kbd>Return</kbd>.

To check if your machine is set up to use something other than Bash,
type `echo $SHELL` in your terminal window.

If your machine is set up to use something other than Bash,
you can run it by opening a terminal and typing `bash`.

[How to Use Terminal on a Mac][mac-terminal]

::::::::::::

:::::::::::: solution

### Linux {#linux2}

The default Unix Shell for Linux operating systems is usually Bash.
On most versions of Linux, it is accessible by running the
[Gnome Terminal][gnome-terminal] or [KDE Konsole][kde-konsole] or [xterm],
which can be found via the applications menu or the search bar.
If your machine is set up to use something other than Bash,
you can run it by opening a terminal and typing `bash`.

::::::::::::

[zip-file]: data/shell-lesson-data.zip
[install_shell]: https://carpentries.github.io/workshop-template/install_instructions/#shell
[wsl]: https://learn.microsoft.com/en-us/windows/wsl/install
[mac-terminal]: https://www.macworld.co.uk/feature/mac-software/how-use-terminal-on-mac-3608274/
[gnome-terminal]: https://help.gnome.org/users/gnome-terminal/stable/
[kde-konsole]: https://konsole.kde.org/
[xterm]: https://en.wikipedia.org/wiki/Xterm



