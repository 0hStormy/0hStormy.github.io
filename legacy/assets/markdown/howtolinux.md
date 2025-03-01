# Desktop Environment

The desktop environment is what makes your comuter have a nice graphical interface, most operating systems have them. Some common desktop environments on Linux include Gnome, KDE Plasma, XFCE, and Cinnamon. Here is what the following look like:

### Gnome

<img src="assets/howtolinux/gnome.png">

### KDE Plasma

<img src="assets/howtolinux/kde.png">

### XFCE

<img src="assets/howtolinux/xfce.png">

### Cinnamon (Linux Mint)

<img src="assets/howtolinux/cinnamon.png">

These images show the defaults of each of the desktop environments. In reality, you can customize these desktops as much as you want to make it work for you. In the end, just look around and see which one is your favorite.

<hr> <id="distro">

# Distributions

A distrobution, or distro for short, is a version of a Linux that company, group, or a single person makes with a specific package manager, desktop environment, and set of applications to make it unique from the rest. Some popular distro's include: Ubuntu, Linux Mint, Fedora, Debian, and Arch.

For beginners, generally Debian based distrobutions such as Ubuntu or Linux Mint are a good start, although feel free to start with anything, I just recommend these because they work well by default and are a little easier to setup.

* **Ubuntu**: Debian based, use `apt`, bi-annual release cycle, uses Gnome desktop by default, stable

* **Linux Mint**: Debian/Ubuntu based, uses `apt`, aims for bi-annual release cycle, uses Cinnamon desktop, stable

* **Debian**: It's own project, uses `apt`, release every 2 years, very stable, adopts standards slower than most Distros

* **Fedora**: It's own project, uses `dnf`, rolling release, uses Gnome desktop by default, stable although adopts new standards quickly

* **Arch**: It's own project, uses `pacman`, rolling release, more on the unstable side, built it yourself Distro, no default desktop

* **NixOS**: It's own project, uses `nix`, rolling release. Very different from the others as everything is setup with config file(s), more info [here](https://github.com/NixOS/nix).

<hr>

# Installing Applications 

There are a couple ways to install software on Linux, mainly you can use a software center, or a package manager. There is also <a href="https://www.winehq.org/">Wine</a> if you need to install Windows programs, but is not super easy to use for new users.

## Software Center

Most popular Linux distros these days have a software center installed to install applications with ease, some examples of software centers include Gnome Software and KDE Discover. Software centers usually support your Distro's packages, Flatpaks, and Snaps.

* Easy for new users to use
* Updates are made simple

## Package Manager

You can also install software, or packages as they're also known in the terminal with a package manager such as `apt`, `dnf`, and `pacman`. As an example, you could do `sudo apt install firefox`, or `sudo pacman -S rust`. Package managers also offer the ability to install system programs if needed, unlike something like Flatpak.

* Installed with your Distro almost no matter what
* System programs and utilities are easier/possible to install

## Flatpak

Flatpaks are a way to install programs that doesn't depend on what Distro you're using, they also are more secure and they simplify the process of publishing applications for developers. To install Flatpak, follow the simple <a href="https://www.flatpak.org/setup/">installation guide</a> for your Distro. And to install an app with Flatpak, you can either use your Software Center, or use the `flatpak` command.

* Distro independent
* Offers Sandboxing for security

## Windows Programs

Although not as easy, you can install windows programs with the Windows compatablility layer known as <a href="https://www.winehq.org/">Wine</a>. Wine is a Windows compatability layer. Wine can a large majority of Windows programs that don't explicitly block it. To use Wine, first check if there is a native Linux version of the program, because it will usually be better. Second, if that's not available, install Wine with their <a href="https://wiki.winehq.org/Download">install guide</a>. Then you will just download the program you want to insttall and install it like a normal Windows program. And if you need any support, google it.

* Compatablility with specific software
* Wine can interact with your native Documents folder

<hr>

# Package Managers

A package manager is a way to install applications or libraries in your terminal, they can also integrate with other apps like a <a href="#software-center">Software Center</a>. They can be used for things as simple as installing something like <a href="https://en.wikipedia.org/wiki/Vim_(text_editor)">Vim</a> to updating your whole system to a new version of your Distro. They work by fetching a list off programs and libraries from repositories, or repos for short. Then it will find where to download that program from the repo and install it.

Here is a list of a few main package managers you will find on Linux and there key differences.

### apt
* Stable
* Easy to use
* Interface can be clunky at times

### dnf
* Easy to use
* Has an easy way to add repos called <a href="https://copr.fedorainfracloud.org/">COPR</a>
* Slower because it always fetches the latest versions of repos

### pacman
* Fast
* Has a bigger learning curve
* Let's you break your system

### nix
* Uses config files to help deal with "Works on my machine 🤓"
* Allows you to restore your system if syou nuke your system
* Could be confusing to a new user
* Distro independent

Overall, it honestly doesn't matter that much what package manager you use, just find one that works for you and stick with it. Be aware that Distro ship specific packages managers, EX: Debian uses `apt`, which means you will be stuck with that package manager.


<hr>

# Gaming

Currently, gaming on Linux is actually pretty usable, I would even say it's better than on MacOS, with issues here and there. A TLDR for this section is if you don't play the newest most advanced games with anticheat, you'll be good for the most part.

## Steam

Steam makes gaming on Linux super easy. Here is a quick step by step guide to setup Steam on Linux.

1. Go to your software center and search for Steam, and click install
2. Open Steam
3. Wait for steam to update
4. Login
5. Go to `Settings > Steam Play > Enable Steam Play for all other titles`
6. Restart Steam
7. Enjoy!

Steam uses a compatability layer called Proton, based on <a href="https://www.winehq.org/">Wine</a>. Proton has a binch of fixes for games specifically so runs really well. It even has some compatability with Easy Anti-Cheat and BattlEye.

## Other games

For other games that aren't on Steam, you can try Lutris or Bottles, which are wrappers for <a href="https://www.winehq.org/">Wine</a> that have installers for other launchers and programs.

For Roblox. The Roblox player with Wine has been blocked, you can still use <a href="https://vinegarhq.org/">Vinegar</a> for Roblox Studio. You should use <a href="https://sober.vinegarhq.org/">Sober</a> for the Roblox player, it is a runtime for the Android version of Roblox. It is closed source but still is a really good program.

<hr>

# Installing

So you're ready to make the plunge? Or maybe you want to try Linux in a Virtual Machine? Let's find out how to install Linux!

**I am not responsible for any damage done to your computer!**

## Real Hardware

First, please **backup ALL of your data!** Because this will wipe your storage drive clean unless you decide to duel-boot, which we will not go into today. Now on real hardware, you need a few things, you need:

* A Computer
* An empty USB flash drive
* An internet connection

Now that you have everything, you will need to choose your <a href="#distrobutions">Distrobution</a>. Once you have chosen that, download the `.iso` file from the Distro's website. Then you use a tool like <a href="https://etcher.balena.io/">Balena Etcher</a> to write the `.iso` file to your USB flash drive. Once you have done that you will plug in your USB flash drive, and then reboot your computer into the temporary boot menu with on of the following keys

* Dell: F12
* HP: Escape
* Lenovo: F12
* Toshiba: F12 or F2
* Gateway: F12
* Other/Custom-Build: Search it up

Once you're in the boot menu, use the arrow keys to choose something along the lines of *"USB HDD"* or *"USB FLASH DRIVE"*, hit `enter` once your found your USB flash drive. It should boot you into <a href="https://en.wikipedia.org/wiki/GNU_GRUB">GRUB</a>, just choose the on along the lines of *"Try or Install `Insert Distro Here`"*.

<img src="assets/howtolinux/grub.png">

Now you should be in <u>Live Mode, which allows you to try Linux without installing it</u>, as it runs off the USB flash drive. It should either **pop-up** wanting to install or there should be a **shortcut** on the desktop to install it. To install, just go through the install process the <a href="#distrobutions">Distro</a>. gives you. Once finished, reboot with the USB flash drive unplugged and you should have a fresh install of the Linux <a href="#distrobutions">Distro</a>. of your choice

*Updated as of 10/6/24*