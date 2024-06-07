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

# Distrobutions

A distrobution, or distro for short, is a version of a Linux that company, group, or a single person makes with a specific package manager, desktop environment, and set of applications to make it unique from the rest. Some popular distro's include: Ubuntu, Linux Mint, Fedora, Debian, and Arch.

For beginners, generally Debian based distrobutions such as Ubuntu or Linux Mint are a good start, although feel free to start with anything, I just recommend these because they work well by default and are a little easier to setup.

* **Ubuntu**: Debian based, use `apt`, bi-annual release cycle, uses Gnome desktop by default, stable

* **Linux Mint**: Debian/Ubuntu based, uses `apt`, aims for bi-annual release cycle, uses Cinnamon desktop, stable

* **Fedora**: It's own project, uses `dnf`, rolling release, uses Gnome desktop by default, stable although adopts new standards quickly

* **Arch**: It's own project, uses `pacman`, rolling release, more on the unstable side, built it yourself Distro, no default desktop

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
* System programs and utilities are a easier to install

## Flatpak

Flatpaks are a way to install programs that doesn't depend on what Distro you're using, they also are more secure and they simplify the process of publishing applications for developers. To install Flatpak, follow the simple <a href="https://www.flatpak.org/setup/">installation guide</a> for your Distro. And to install an app with Flatpak, you can either use your Software Center, or use the `flatpak` command.

* Distro independent
* Offers Sandboxing

## Windows Programs

Although not as easy, you can install windows programs with the Windows compatablility layer known as <a href="https://www.winehq.org/">Wine</a>. WIne is a Widow compatability layer that has been under development for over 20 years, it can run most Windows programs that don't explicitly block it. To use Wine, first check if there is a native Linux version of the program, because it will usually be better. Second, if that's not available, install Wine with their <a href="https://wiki.winehq.org/Download">install guide</a>. Then you will just download the program you want to insttall and install it like a normal Windows program. And if you need any support, google it.

* Compatablility with specific software
* WIndows programs won't mess with the rest of your system

<hr>

# Installing

So you're ready to make the plunge? Or maybe you want to try Linux in a Virtual Machine? Let's find out how to install Linux!

## Real Hardware

First, please **backup ALL of your data!** Because this will wipe your storage drive clean unless you decide to duel-boot, which we will not go into today. Now on real hardware, you need a few things, you need:

* A Computer
* An empty USB flash drive
* An internet connection

Now that you have everything, you will need to choose your <a href="distro">Distrobution</a>