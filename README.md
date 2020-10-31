# <div align="center">Awesome-BSD-PPP</div>
###### <div align="center">Port, Programs, and Projects! </div>

***********

![BSD Banner](img/BSDGitLogo.png)

***********

This repository will function as a list of interesting ports, programs, and Projects for newbies and veterans to BSD.

**Acknowledgements**:
I am merely a passionate newbie to these OS's and freely admit that I know enough to be dangerous, please put in a pull request if you find information that can be improved or otherwise modified to be clearer.

## Table of Contents

- [Frequenty Asked Questions](#FAQ)
    - [What is BSD?](#What-is-BSD?)
    - [How is BSD different than Linux?](#How-is-BSD-different-than-Linux?)
    - [What are the differences between Packages and Ports?](#What-are-the-differences-between-Packages-and-Ports?)
    - [Can I mix and Match Ports and Packages?](#Can-I-mix-and-Match-Ports-and-Packages?)
    - [What if I have another BSD?](What-if-I-have-another-BSD?)
- [Ports and Programs](#Ports-and-Programs)
    - [Audio](#Audio)
    - [UNIX Shells](#UNIX-Shells)
- [Projects](#Projects)
- [How-To's](#How-To's)
- [Attribution](#Attribution)


## FAQ

#### What is BSD?

![Awesome][UNIX tree]

BSD was originally a UNIX based operating system that was developed at the the University of Berkeley in California in the late 70's. At the time it was a closed source, or partially closed source operating system that was gradually re-engineered into a completely Open source Operating System now used all over the world.

#### How is BSD different than Linux?

BSD takes a more centralized approach in its development having entire program and kernel ecosystems developed together. Whereas Linux itself is just a kernel which then requires groups of people to add packages and other system components together to build the whole operating system, this creates a Linux "Distribution" a distribution of software components (programs, Kernel, drivers and whatnot.)

Because of this difference and because BSD is built around an entire ecosystem from the start, it has an excellent history of documentation for its various functions, both in the Kernel, and with its programs.

For the average UNIX user, it will seem very familiar in many ways, and learning BSD from Linux or other UNIX based Operating Systems will be fairly straightforward, with nearly all of the most common UNIX friendly tools and shells are available for the user.

#### What are the differences between Packages and Ports?

A ***Package*** (Referred to as a program in this list) is a program already compiled into a binary that can be run on the largest number of systems due to be pre-compiled for you with the most general settings. It requires only the briefest installation, and does not require compilation to run on your machine.

A ***Port*** is source code with instructions that allow you to compile the code on your machine to create an executable program. It has the advantage of allowing you to compile the program in a more specific way for your machine to get extra performance from the code or only get parts of the program that you need such as only getting the webhost part of an Apache webserver, but no WebDAV or support for User Directories making the program smaller and leaner.

BSD allows installation of both types of software to allow for either ease or flexibility in your OS and environment, it is up to you to decide which you would prefer to use.

#### Can I mix and Match Ports and Packages?

If you know what you are doing, there should be little issue, Issues come when you don't know.

A basic scenario would be this: say you would like to install only part of a webserver, and you modify the port make file to ensure you only install that part. It will function normally, but if you install a program that requires that as a dependency, it may see it, but malfunction due to not having the entirely of that program installed. If the software have no relation to each other, there should be no issues. But when in doubt, install either only ports, or only Packages.

#### What if I have another BSD?

If you use MidnightBSD, NomadBSD or GhostBSD, or any of a variety of alternative BSD's, typically they are based off one of the main 4 BSD's: DragonflyBSD, FreeBSD, NetBSD, or OpenBSD and will have access to their ports. A brief perusal of the BSD's home website will generally inform you of which you can use. Simply click on the BSD that yours is based on here and follow the same instructions.

Debian GNU/kFreeBSD does not have a port system, and instead uses the Debian Packaging that Debian Linux uses.

***********

## Ports and Programs

### Audio

- [![Open-Source Software][OSS Icon]](https://github.com/audacity/audacity) [Audacity](http://www.audacityteam.org/) - Free, open source, cross-platform software for recording and editing sounds.

 [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/audio/audacity/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/audio/audacity) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/audio/audacity) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/audio/audacity)

 ### UNIX Shells

- [![Open-Source Software][OSS Icon]](https://github.com/tcsh-org/tcsh) [csh](https://www.tcsh.org/) - The C Shell or csh is the default Shell in NetBSD and OpenBSD, It was written by Bill Joy in the late 70's and is one of the oldest continuously developed shells. Development has transferred entirely to tcsh.

[![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/44bsd-csh/) ![Available in NetBSD](img/netbsdico.png) ![Available in DragonflyBSD](img/dragonflybsdico.png) ![Available in OpenBSD](img/openbsdico.png) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://savannah.gnu.org/projects/bash/) [Bash](https://www.gnu.org/software/bash/) - The GNU Bourne-Again SHell or bash shell, is typically the default shell available on Linux distributions is available for BSD also, it supports advanced scripting features and is very extensible. Highly reccomended for people trying BSD to ease transition into the OS.

    [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/bash/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/bash) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/bash) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/bash) ![](img/termprog.png)

    - [![Open-Source Software][OSS Icon]](https://github.com/ohmybash/oh-my-bash) [Oh-My-Bash](https://ohmybash.nntoan.com/) - Oh My Zsh is an open source, community-driven framework for managing your zsh configuration. Can be installed via git or shellscript if not in Ports.

    ![](img/termprog.png)
<br/>

- [![Open-Source Software][OSS Icon]](https://github.com/fish-shell/fish-shell) [Fish](https://fishshell.com/) - Fish is a shell designed with user friendliness in mind, having many included features such as syntax highlighting and autosuggestions, with extensive tab autocompletion, it is a very interesting take on a POSIX shell.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/fish/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/fish) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/fish) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/fish)  ![](img/termprog.png)

   - [![Open-Source Software][OSS Icon]](https://github.com/oh-my-fish/oh-my-fish) [Oh-My-Fish](https://github.com/oh-my-fish/oh-my-fish) - Oh My Fish is an open source, framework which allows for the installation of plugins that extend the functionality of fish. Can be installed via git or shellscript.

   ![](img/termprog.png)
<br/>

- [![Open-Source Software][OSS Icon]](https://github.com/tcsh-org/tcsh) [tcsh](https://www.tcsh.org/) - tcsh is the continuation and successor to csh and expands on its functionalities and capabilities. It is the default root shell on FreeBSD, and can be installed on the other four major BSD's.

   ![Available in FreeBSD](img/freebsdico.png) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/tcsh) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/tcsh) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/tcsh)  ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](http://zsh.sourceforge.net/Arc/source.html) [Zsh](http://zsh.sourceforge.net/) - Zsh is an extension of the Bourne Shell (bsh) and includes many improvements such as autocorrect, autocompletion, and is extensible with a great deal of many features. It is the Default Shell on MacOS.

    [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/zsh/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/zsh) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/zsh) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/zsh) ![](img/termprog.png)

    - [![Open-Source Software][OSS Icon]](https://github.com/ohmyzsh/ohmyzsh/) [Oh-My-Zsh](https://ohmyz.sh/) - Oh My Zsh is an open source, community-driven framework for managing your zsh configuration. Can be installed via git shellscript if not in Ports.

       [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/ohmyzsh/) ![](img/termprog.png)
<br/>

***********

## Projects

***********

## How-To's

- [How to install Ports in DragonflyBSD](https://www.dragonflybsd.org/docs/howtos/HowToDPorts/) - From the official DragonflyBSD Docs
- [How to install Ports in FreeBSD](https://www.freebsd.org/doc/handbook/ports-using.html) - From the official FreeBSD Docs.
- [How to install Ports in NetBSD](https://www.netbsd.org/docs/pkgsrc/using.html) - From the official NetBSD Docs.
- [How to install Ports in OpenBSD](https://www.openbsd.org/faq/ports/ports.html) - From the official OpenBSD FAQs.

***********

## Attribution:
*The usage of the BSD Family Tree in the What is BSD FAQ is used under the GNU Free Documentation License Version 1.2 or later. All logos of the various BSD's are the property of their respective projects.*

[UNIX tree]: https://upload.wikimedia.org/wikipedia/commons/7/77/Unix_history-simple.svg
[OSS Icon]: https://svgshare.com/i/R6P.svg
[Money Icon]: https://svgshare.com/i/R6N.svg
