# <div align="center">Awesome-BSD-PPP</div>
###### <div align="center">Port, Programs, and Projects! </div>

***********

![BSD Banner](img/BSDGitLogo.png)

***********

This repository will function as a list of interesting ports, programs, and Projects for newbies and veterans to BSD.

**Acknowledgements**:
I am merely a passionate newbie to these OS's and freely admit that I know enough to be dangerous, please put in a pull request if you find information that can be improved or otherwise modified to be clearer.

## Table of Contents

- [Icon Key](#Key)
- [Frequenty Asked Questions](#FAQ)
    - [What is BSD?](#What-is-BSD?)
    - [How is BSD different than Linux?](#How-is-BSD-different-than-Linux?)
    - [What are the differences between Packages and Ports?](#What-are-the-differences-between-Packages-and-Ports?)
    - [Can I mix and Match Ports and Packages?](#Can-I-mix-and-Match-Ports-and-Packages?)
    - [What if I have another BSD?](What-if-I-have-another-BSD?)
    - [How can I install these programs?](How-can-I-install-these-programs?)
    - [What are the Big Four BSD's?](What-are-the-Big-Four-BSD's?)
- [Ports and Programs](#Ports-and-Programs)
    - [Audio](#Audio)
    - [Desktop Environments](#Desktop-Environments)
    - [Security](#Security)
    - [UNIX Shells](#UNIX-Shells)
- [Projects](#Projects)
- [How-To's](#How-To's)
- [Other Awesome Lists](#Other-Awesome-Lists)
- [Attribution](#Attribution)

## Key
  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/bash/) = is available in the FreeBSD Ports, provides a link to that port.

  [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/bash) = is available in the NetBSD Ports, provides a link to that port.

  [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/bash) = is available in the DragonflyBSD Ports, provides a link to that port.

  [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/bash) = is available in the OpenBSD Ports, provides a link to that port.

  [![Terminal Program](img/termprog.png)](https://en.wikipedia.org/wiki/Command-line_interface) = Program is Command line only.

  ![Open-Source Software][OSS Icon] = Program is open source, and is freely available, source code and all.

  ![Closed-Source Software][Money Icon] = Program is closed source, and may cost money.

## FAQ

#### What is BSD?

![Awesome][UNIX tree]

BSD was originally a UNIX based operating system that was developed at the the University of Berkeley in California in the late 70's. At the time it was a closed source, or partially closed source operating system that was gradually re-engineered into a completely Open source Operating System now used all over the world.

#### How is BSD different than Linux?

BSD takes a more centralized approach in its development having entire program and kernel ecosystems developed together. Whereas Linux itself is just a kernel which then requires groups of people to add packages and other system components together to build the whole operating system, this creates a Linux "Distribution" a distribution of software components (programs, Kernel, drivers and whatnot.)

Because of this difference and because BSD is built around an entire ecosystem from the start, it has an excellent history of documentation for its various functions, both in the Kernel, and with its programs.

For the average UNIX user, it will seem very familiar in many ways, and learning BSD from Linux or other UNIX based Operating Systems will be fairly straightforward, with nearly all of the most common UNIX friendly tools and shells are available for the user.

#### What are the differences between Packages and Ports?
<div align="center">

![](img/ports.jpg)
</div>

A ***Package*** (Referred to as a program in this list) is a program already compiled into a binary that can be run on the largest number of systems due to be pre-compiled for you with the most general settings. It requires only the briefest installation, and does not require compilation to run on your machine.

A ***Port*** is source code with instructions that allow you to compile the code on your machine to create an executable program. It has the advantage of allowing you to compile the program in a more specific way for your machine to get extra performance from the code or only get parts of the program that you need such as only getting the webhost part of an Apache webserver, but no WebDAV or support for User Directories making the program smaller and leaner.

BSD allows installation of both types of software to allow for either ease or flexibility in your OS and environment, it is up to you to decide which you would prefer to use.

#### Can I mix and Match Ports and Packages?

If you know what you are doing, there should be little issue, Issues come when you don't know.

A basic scenario would be this: say you would like to install only part of a webserver, and you modify the port make file to ensure you only install that part. It will function normally, but if you install a program that requires that as a dependency, it may see it, but malfunction due to not having the entirely of that program installed. If the software have no relation to each other, there should be no issues. But when in doubt, install either only ports, or only Packages.

#### What if I have another BSD?

If you use MidnightBSD, NomadBSD or GhostBSD, or any of a variety of alternative BSD's, typically they are based off one of the main 4 BSD's: DragonflyBSD, FreeBSD, NetBSD, or OpenBSD and will have access to their ports. A brief perusal of the BSD's home website will generally inform you of which you can use. Simply click on the BSD that yours is based on here and follow the same instructions.

Debian GNU/kFreeBSD does not have a port system, and instead uses the Debian Packaging that Debian Linux uses.

#### How can I install these programs?

It depends on the BSD but they all will be somewhat similar, this will assume that you have the OS setup and are sitting at a command line. These will nearly always have to be run as the super user or root.

**DragonflyBSD**: pkg install (*packagename*)
**FreeBSD**: pkg install (*packagename*)
**NetBSD**: pkgin install (*packagename*)
  ^*Note that NetBSD may need to have [pkgin installed](https://pkgin.net/) first before this command will function.*
**OpenBSD**: pkg_add (*packagename*)

#### What are the Big Four BSD's?

Currently there are 4 BSD projects seen as the largest among the BSD's and are the various icons listed here, for those who are not familiar with one, in alphabetical order here are some basic descriptions of them:

#####[DragonflyBSD](https://www.dragonflybsd.org/)

<div align="center">

![](img/DragonflyBSD.png)
</div>

DragonFly belongs to the same class of operating systems as other BSD-derived systems and Linux. It is based on the same UNIX ideals and APIs and shares ancestor code with other BSD operating systems. DragonFly provides an opportunity for the BSD base to grow in an entirely different direction from the one taken in the FreeBSD, NetBSD, and OpenBSD series.

#####[FreeBSD](https://www.freebsd.org/)

<div align="center">

![](img/freeBSD.png)
</div>

FreeBSD is an operating system used to power modern servers, desktops, and embedded platforms. A large community has continually developed it for more than thirty years. Its advanced networking, security, and storage features have made FreeBSD the platform of choice for many of the busiest web sites and most pervasive embedded networking and storage devices.

#####[NetBSD](https://www.netbsd.org/)

<div align="center">

![](img/netBSD.png)
</div>

NetBSD is a free, fast, secure, and highly portable Unix-like Open Source operating system. It is available for a wide range of platforms, from large-scale servers and powerful desktop systems to handheld and embedded devices.

#####[OpenBSD](https://www.openbsd.org/)

<div align="center">

![](img/openbsd.png)
</div>

The OpenBSD project produces a FREE, multi-platform 4.4BSD-based UNIX-like operating system. Our efforts emphasize portability, standardization, correctness, proactive security and integrated cryptography. As an example of the effect OpenBSD has, the popular OpenSSH software comes from OpenBSD.

***********

## Ports and Programs

### Audio

- [![Open-Source Software][OSS Icon]](https://github.com/audacity/audacity) [Audacity](http://www.audacityteam.org/) - Free, open source, cross-platform software for recording and editing sounds.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/audio/audacity/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/audio/audacity) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/audio/audacity) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/audio/audacity)

- [![Open-Source Software][OSS Icon]](https://github.com/clementine-player/Clementine) [Clementine](https://www.clementine-player.org/) - Clementine is a multiplatform music player. It is inspired by Amarok 1.4, focusing on a fast and easy-to-use interface for searching and playing your music.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/audio/clementine-player/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/wip/clementine) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/wip/clementine) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/audio/clementine)

### Desktop Environments

- [![Open-Source Software][OSS Icon]](https://gitlab.gnome.org/GNOME/gnome-shell) [Gnome 3](https://www.gnome.org/gnome-3/) - GNOME 3 provides a focused working environment that helps you to get things done, and it is packed with features that will make you more productive. A powerful search feature lets you access all your work from one place. Side-by-side windows makes it easy to view several documents at the same time.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/x11/lumina/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/wip/lumina) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/wip/lumina) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/x11/lumina)

- [![Open-Source Software][OSS Icon]](https://github.com/KDE) [KDE](https://kde.org/) - K Desktop Environment (KDE) is an Open Source graphical desktop environment for UNIX workstations. Initially called the Kool Desktop Environment it includes a file manager, a window manager, a help system, a configuration system, tools and utilities, and several applications.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/x11/kde5/) [![Available in NetBSD](img/netbsdico.png)](https://ftp.netbsd.org/pub/pkgsrc/current/pkgsrc/x11/kde-workspace4/README.html) [![Available in DragonflyBSD](img/dragonflybsdico.png)](ftp://muug.ca/mirror/dragonflybsd/dports/dragonfly%3A5.10%3Ax86%3A64/LATEST/All/kde5-5.19.5.20.08.1.txz) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/x11/kde)

- [![Open-Source Software][OSS Icon]](https://github.com/lumina-desktop/lumina) [Lumina](https://lumina-desktop.org/) - The Lumina desktop is designed to be fast, customizable, flexible, and lightweight. Lumina works great in multi-monitor configurations and with high-resolution monitors as well as single-screen configurations on laptops or tablets.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/x11/lumina/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/wip/lumina) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/wip/lumina) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/x11/lumina)

### Security

- [![Open-Source Software][OSS Icon]](https://github.com/BastilleBSD/bastille) [Bastille](https://bastillebsd.org/) - Bastille is an open-source system for automating deployment and management of containerized applications on FreeBSD.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/sysutils/bastille/) ![](img/termprog.png)

### UNIX Shells

- [![Open-Source Software][OSS Icon]](https://savannah.gnu.org/projects/bash/) [Bash](https://www.gnu.org/software/bash/) - The GNU Bourne-Again SHell or bash shell, is typically the default shell available on Linux distributions is available for BSD also, it supports advanced scripting features and is very extensible. Highly reccomended for people trying BSD to ease transition into the OS.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/bash/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/bash) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/bash) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/bash) ![](img/termprog.png)

  - [![Open-Source Software][OSS Icon]](https://github.com/ohmybash/oh-my-bash) [Oh-My-Bash](https://ohmybash.nntoan.com/) - Oh My Zsh is an open source, community-driven framework for managing your zsh configuration. Can be installed via git or shellscript if not in Ports.

    ![](img/termprog.png)
<br/>

- [![Open-Source Software][OSS Icon]](https://github.com/tcsh-org/tcsh) [csh](https://www.tcsh.org/) - The C Shell or csh is the default Shell in NetBSD and OpenBSD, It was written by Bill Joy in the late 70's and is one of the oldest continuously developed shells. Development has transferred entirely to tcsh.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/44bsd-csh/) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://github.com/elves/elvish) [Elvish](https://elv.sh/) - Elvish is a friendly interactive shell and an expressive programming language. It runs on Linux, BSDs, macOS and Windows. Despite its pre-1.0 status, it is already suitable for most daily interactive use.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/elvish/) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/elvish)  ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://github.com/fish-shell/fish-shell) [Fish](https://fishshell.com/) - Fish is a shell designed with user friendliness in mind, having many included features such as syntax highlighting and autosuggestions, with extensive tab autocompletion, it is a very interesting take on a POSIX shell.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/fish/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/fish) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/fish) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/fish)  ![](img/termprog.png)

   - [![Open-Source Software][OSS Icon]](https://github.com/oh-my-fish/oh-my-fish) [Oh-My-Fish](https://github.com/oh-my-fish/oh-my-fish) - Oh My Fish is an open source, framework which allows for the installation of plugins that extend the functionality of fish. Can be installed via git or shellscript.

      ![](img/termprog.png)
<br/>

- [![Open-Source Software][OSS Icon]](https://github.com/tcsh-org/tcsh) [tcsh](https://www.tcsh.org/) - tcsh is the continuation and successor to csh and expands on its functionalities and capabilities. It is the default root shell on FreeBSD, and can be installed on the other four major BSD's.

   ![Available in FreeBSD](img/freebsdico.png) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/tcsh) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/tcsh) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/tcsh)  ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](http://zsh.sourceforge.net/Arc/source.html) [Zsh](http://zsh.sourceforge.net/) - Zsh is an extension of the Bourne Shell (bsh) and includes many improvements such as autocorrect, autocompletion, and is extensible with a great deal of many features. Theming is very popular with Zsh. It is the Default Shell on MacOS.

    [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/zsh/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/zsh) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/zsh) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/zsh) ![](img/termprog.png)

    - [![Open-Source Software][OSS Icon]](https://github.com/ohmyzsh/ohmyzsh/) [Oh-My-Zsh](https://ohmyz.sh/) - Oh My Zsh is an open source, community-driven framework for managing your zsh configuration and themes. Can be installed via git shellscript if not in Ports.

      [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/ohmyzsh/) ![](img/termprog.png)
<br/>

***********

## Projects

*Links here are to projects that use the BSD OS in some capacity, Firewalls, Webservers, Gameservers, you name it!*

***********

## How-To's

- [How to install Ports in DragonflyBSD](https://www.dragonflybsd.org/docs/howtos/HowToDPorts/) - From the official DragonflyBSD Docs
- [How to install Ports in FreeBSD](https://www.freebsd.org/doc/handbook/ports-using.html) - From the official FreeBSD Docs.
- [How to install Ports in NetBSD](https://www.netbsd.org/docs/pkgsrc/using.html) - From the official NetBSD Docs.
- [How to install Ports in OpenBSD](https://www.openbsd.org/faq/ports/ports.html) - From the official OpenBSD FAQs.

***********

## Other Awesome Lists

*Other Awesome BSD lists that can shed light on other parts of BSD.*

- [Awesome BSD](https://github.com/DiscoverBSD/awesome-bsd) - Covers mainly BSD OS variants, and groups to discuss BSD with across social media.

***********

## Attribution:
*The usage of the BSD Family Tree in the What is BSD FAQ is used under the GNU Free Documentation License Version 1.2 or later. All logos of the various BSD's are the property of their respective projects.*

[UNIX tree]: https://upload.wikimedia.org/wikipedia/commons/7/77/Unix_history-simple.svg
[OSS Icon]: https://svgshare.com/i/R6P.svg
[Money Icon]: https://svgshare.com/i/R6N.svg
