# Mac OS X Development Setup

Basic Development Setup including Chrome, iTerm2, Atom, Hombrew, Git, and Node.

This article assumes your computer:

- Is running Mac OS X 10.12 El Capitan or above
- Is virus and malware free
- Uses the latest, stable version of its operating system
- Has a functioning screen, keyboard, and trackpad
- Has plenty of free hard drive space and memory
- Can reliably connect to wireless networks

## Getting Started

Save all files you may have open and close all other applications. (If you are at home and want to make a backup of your computer just in case, now would be the time).

Make sure that you have your computer username and password memorized or handy and that you are the admin (or root) user for the computer (more help with user types [here](https://support.apple.com/kb/PH21994?locale=en_US)).

## Mac OS X Updates

Before we dive in to modifications, open the AppStore application and check if you have any updates -- unless you are sure you don't need them, just accept all updates. This may take some time to download and install, but it is important to be starting with the most up to date operating system and tools.

### Xcode
From the AppStore, search for and install Xcode.

When you're done, if it's not already required, reboot your computer.

Checklist:

* Updated to the latest version of Mac OS X
* Installed/Updated Xcode from the AppStore
* Run all updates from the AppStore
* Restarted your computer

## Chrome

Now it's time to install Google Chrome, a fast and free web browser that automatically updates itself with the latest web technologies.

[Download Chrome](https://www.google.com/chrome/browser/desktop/), open the disk image file, and drag the app icon into your `/Applications` folder.

**PROPROTIP:** Allow Chrome to become your default browser.

Firefox Developer Edition is also a solid choice for developers, but I prefer Chrome.

Navigate to the `Chrome > Preferences` -- scroll to the bottom of the page and click the **Show advanced settings...** link. Scroll down a bit more until you find the **Send a "Do Not Track" request with your browser traffic** and check the box.

**PROTIP:** You may want to consider installing an [ad blocking extension](https://chrome.google.com/webstore/detail/adblock/gighmmpiobklfepjocnamgkkbiglidom) to Chrome.

### Other Helpful Chrome Extensions

Dev Related:
* AdBlock
* Block Site
* Personal Blocklist
* Pesticide for Chrome
* JSONView

Other:
* Kill News Feed
* Momentum


## iTerm2 

There are many different options to customize your terminal application, however, I recommend using iTerm2 instead.

Download and install [iTerm2](https://www.iterm2.com/)

OPTIONAL: You can customize the look of iTerm from the preferences menu OR follow this guide to [install z shell and oh-my-zsh](https://github.com/thacherT1D/fishToZsh) for even more functionality.


## Atom

Now it's time to install [Atom](https://atom.io/), a hackable text editor for the 21st century.

To get started, [download Atom](https://atom.io/download/mac), unzip the archive file, and drag the app icon into your `/Applications` folder. Double click to open atom.

Close any tabs by pressing `Command` + `W`. Then, navigate to the `Atom > Preferences` menu item by pressing the `Command` + `,` .

Under the **Settings** tab, in the **Editor Settings** section, change the following:

| Name                               | Value              |
|------------------------------------|--------------------|
| Font Family                        | Menlo              |
| Font Size                          | 18                 |
| Show Indent Guide                  | Checked            |

Under the **Install** tab, with the **Package** button highlighted, install the following:

| Name                           | Type    |
|--------------------------------|---------|
| file-icons                     | Package |
| language-fish-shell            | Package |

Under the **Install** tab, with the **Themes** button highlighted, install the following:

| Name                           | Type         |
|--------------------------------|--------------|
| tomorrow-night-eighties-syntax | Syntax Theme |

Under the **Packages** tab search for autosave -- under **Core Packages** click the **Settings** button, in the **Settings** section check Enabled.

When you're done, close the preferences tab by pressing `Command` + `W`.

### Install the Shell Commands

You'll find it insanely useful to open files and directories into Atom from the Terminal.

To get started, select the `Atom > Install Shell Commands` menu item.


## Homebrew

Now that your Terminal is setup, it's time to install [Homebrew](http://brew.sh/), the de facto package manager for OS X. If you've never heard of a package manager, think of it as an app store for **free** command line programs.

To get started, run the following command in your shell. It'll download and run a script file that downloads and installs Homebrew onto your development environment.

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

If asked, be sure to agree when asked to install the **Xcode CommandLine Tools**. It may take about 10 minutes to download and install.


### Update Homebrew

If you've previously installed Homebrew, now's a good time to update it by running the following command.

```
brew update
```

If it's been a while since the last update, you'll see something like this.

**PROTIP:** Run this command periodically as Homebrew doesn't automatically update itself.

### Verify Homebrew

To verify Homebrew is installed correctly, run the following command.

```
brew doctor
```

## Git

Using Homebrew, you can also install [Git](https://git-scm.com/), the version control system of choice among choosy developers.

To get started, run the following command.

```
brew install git
```

Once it finishes, run the following command.

```
git --version
```

Let's configure Git to sign your commits with your name and email address.

**WARNING:** Before running the following commands, replace `YOUR FULL NAME` and `YOUR EMAIL ADDRESS` with the name and email from [your GitHub account](https://github.com/settings/profile).

```
git config --global user.name 'YOUR FULL NAME'
git config --global user.email 'YOUR EMAIL ADDRESS'
```

## Node

Using Homebrew, you can also install [Node](https://nodejs.org/), an open-source, cross-platform runtime system for developing applications in JavaScript. In other words, it runs JavaScript outside the browser.

To get started, run the following command.

```
brew install node
```

Once it finishes, run the following command.

```
node -v
```

## Congratulations!

You've successfully setup a web development environment on Mac OS X!

### Other Useful Dev Tools
These are a few other tools that can be helpful for different aspects of development:
* Password Manager: [Last Pass](https://lastpass.com) or [One Password](https://1password.com/)
* Organizes windows on your screen: [Spectacle](https://www.spectacleapp.com/) OR [Moom](https://manytricks.com/moom/)
* Keeps a history of what you copy [Jump Cut](http://jumpcut.sourceforge.net/)
* Color Picker: [sip](http://sipapp.io/) (color)
* Image Editor: [Pixelmaker](http://www.pixelmator.com/mac/)
* Color Schemes: [Coolors](https://coolors.co/)
* For Notes: [One Note](https://www.onenote.com/) OR [Evernote](https://evernote.com/)
* Automatically dim your screen for working at night: [Flux](https://justgetflux.com/) — night time your screen
* Level up your screenshots: [SnappyApp](https://snappy-app.com/)
* Take notes with a live MarkDown preview [MacDown](https://macdown.uranusjr.com/)
