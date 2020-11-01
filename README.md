# <div align="center">Awesome-BSD-PPP</div>


***********

![BSD Banner](img/BSDGitLogo.png)

***********

###### <div align="center">Port, Programs, and Projects! </div>

This repository will function as a list of interesting ports, programs, and Projects for newbies and veterans to BSD.

**Acknowledgements**:
I am merely a passionate newbie to these OS's and freely admit that I know enough to be dangerous, please put in a pull request if you find information that can be improved or otherwise modified to be clearer.

## Table of Contents

- [Frequenty Asked Questions](#FAQ)
  - [What is BSD?](#What-is-BSD?)
  - [How is BSD different than Linux?](#How-is-BSD-different-than-Linux?)
  - [What are the differences between Packages and Ports?](#What-are-the-differences-between-Packages-and-Ports?)
  - [Can I mix and Match Ports and Packages?](#Can-I-mix-and-Match-Ports-and-Packages)
  - [What if I have another BSD?](#What-if-I-have-another-BSD)
  - [How can I install these programs?](#How-can-I-install-these-programs)
  - [What are the Big Four BSD's?](#What-are-the-Big-Four-BSD's)
- [Icon Key](#Key)
- [Ports and Programs](#Ports-and-Programs)
  - [Audio](#Audio)
  - [Command Line Utilities](#Command-Line-Utilities)
  - [Data Backup and Recovery](#Data-Backup-and-Recovery)
  - [Desktop Environments](#Desktop-Environments)
  - [Emulators](#Emulators)
  - [File Managers](#File-Managers)
  - [Network Tools](#Network-Tools)
  - [Office](#Office)
  - [Security](#Security)
  - [Terminal Emulators](#Terminal-Emulators)
  - [UNIX Shells](#UNIX-Shells)
  - [Utilites](#Utilities)
- [Projects](#Projects)
- [How-To's](#How-To's)
- [Other Awesome Lists](#Other-Awesome-Lists)
- [Attribution](#Attribution)
- [Miscallaneous Web Sources](#Miscallaneous-Web-Sources)

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

It depends on the BSD but they all will be somewhat similar, this will assume that you have the OS setup and are sitting at a command line. These will nearly always have to be run as the super user or root. (Using the doas or sudo commands.)

**DragonflyBSD**: pkg install (*packagename*)

**FreeBSD**: pkg install (*packagename*)

**NetBSD**: pkgin install (*packagename*)
  ^*Note that NetBSD may need to have [pkgin installed](https://pkgin.net/) first before this command will function.*

**OpenBSD**: pkg_add (*packagename*)

#### What are the Big Four BSD's?

Currently there are 4 BSD projects seen as the largest among the BSD's and are the various icons listed here, for those who are not familiar with one, in alphabetical order here are some basic descriptions of them:

<div align="center">

# [DragonflyBSD](https://www.dragonflybsd.org/)

![](img/DragonflyBSD.png)
</div>

DragonFly belongs to the same class of operating systems as other BSD-derived systems and Linux. It is based on the same UNIX ideals and APIs and shares ancestor code with other BSD operating systems. DragonFly provides an opportunity for the BSD base to grow in an entirely different direction from the one taken in the FreeBSD, NetBSD, and OpenBSD series.

<div align="center">

# [FreeBSD](https://www.freebsd.org/)

![](img/FreeBSD.png)
</div>

FreeBSD is an operating system used to power modern servers, desktops, and embedded platforms. A large community has continually developed it for more than thirty years. Its advanced networking, security, and storage features have made FreeBSD the platform of choice for many of the busiest web sites and most pervasive embedded networking and storage devices.

<div align="center">

# [NetBSD](https://www.netbsd.org/)

![](img/NetBSD.png)
</div>

NetBSD is a free, fast, secure, and highly portable Unix-like Open Source operating system. It is available for a wide range of platforms, from large-scale servers and powerful desktop systems to handheld and embedded devices.

<div align="center">

# [OpenBSD](https://www.openbsd.org/)

![](img/openbsd.png)
</div>

The OpenBSD project produces a FREE, multi-platform 4.4BSD-based UNIX-like operating system. Our efforts emphasize portability, standardization, correctness, proactive security and integrated cryptography. As an example of the effect OpenBSD has, the popular OpenSSH software comes from OpenBSD.

***********

## Key
  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/bash/) = is available in the FreeBSD Ports, and provides a link to that port.

  [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/bash) = is available in the NetBSD Ports, and provides a link to that port.

  [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/bash) = is available in the DragonflyBSD Ports, and provides a link to that port.

  [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/bash) = is available in the OpenBSD Ports, and provides a link to that port.

  [![Terminal Program](img/termprog.png)](https://en.wikipedia.org/wiki/Command-line_interface) = Program is Command line only.

  ![Open-Source Software][OSS Icon] = Program is open source, and is freely available, source code and all. if you click this icon, it will take you to that source code for that program.

  ![Closed-Source Software][Money Icon] = Program is closed source, and may cost money.

***********

## Ports and Programs

### Audio

- [![Open-Source Software][OSS Icon]](https://github.com/audacity/audacity) [Audacity](http://www.audacityteam.org/) - Free, open source, cross-platform software for recording and editing sounds.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/audio/audacity/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/audio/audacity) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/audio/audacity) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/audio/audacity)

- [![Open-Source Software][OSS Icon]](https://github.com/clementine-player/Clementine) [Clementine](https://www.clementine-player.org/) - Clementine is a multiplatform music player. It is inspired by Amarok 1.4, focusing on a fast and easy-to-use interface for searching and playing your music.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/audio/clementine-player/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/wip/clementine) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/wip/clementine) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/audio/clementine)

### Command Line Utilities

- [![Open-Source Software][OSS Icon]](https://sourceforge.net/projects/anacron/) [Anacron](https://sourceforge.net/projects/anacron/) - Anacron is a periodic command scheduler. It executes commands at intervals specified in days. Unlike cron, it does not assume that the system is running continuously. It can therefore be used to control the execution of daily, weekly and monthly jobs (or anything with a period of n days), on systems that don't run 24 hours a day. When installed and configured properly, Anacron will make sure that the commands are run at the specified intervals as closely as machine-uptime permits.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/sysutils/anacron/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/time/anacron) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/time/anacron) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/sysutils/anacron) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://github.com/athityakumar/colorls) [Colorls](https://github.com/athityakumar/colorls) - A Ruby gem that beautifies the terminal's ls command, with color and font-awesome icons. 🎉

  [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/misc/colorls) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/misc/colorls) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/sysutils/colorls) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](http://mama.indstate.edu/users/ice/tree/) [Colortree](http://mama.indstate.edu/users/ice/tree/) - Tree is a recursive directory listing command that produces a depth indented listing of files, which is colorized ala dircolors if the LS_COLORS environment variable is set and output is to tty. Tree has been ported and reported to work under the following operating systems: Linux, FreeBSD, OS X, Solaris, HP/UX, Cygwin, HP Nonstop and OS/2.

  [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/sysutils/colortree) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://github.com/ogham/exa) [Exa](https://the.exa.website/) - exa is an improved file lister with more features and better defaults. It uses colours to distinguish file types and metadata. It knows about symlinks, extended attributes, and Git. And it’s small, fast, and just one single binary.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/sysutils/exa/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/sysutils/exa) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/sysutils/exa) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/sysutils/exa) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://github.com/dylanaraps/neofetch) [Neofetch](https://github.com/dylanaraps/neofetch) - Neofetch is a command-line system information tool written in bash 3.2+. Neofetch displays information about your operating system, software and hardware in an aesthetic and visually pleasing way.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/sysutils/neofetch/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/sysutils/neofetch) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/sysutils/neofetch) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/sysutils/neofetch) ![](img/termprog.png)

### Data Backup and Recovery

- [![Open-Source Software][OSS Icon]](https://www.bacula.org/git/cgit.cgi/bacula/) [Bacula - Client](https://www.bacula.org/) - Bacula is a set of Open Source, computer programs that permit you to manage backup, recovery, and verification of computer data across a network of computers of different kinds. This is for the client installation.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/sysutils/bacula9-client/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/sysutils/bacula-clientonly) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/sysutils/bacula-clientonly) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/sysutils/bacula)

- [![Open-Source Software][OSS Icon]](https://www.bacula.org/git/cgit.cgi/bacula/) [Bacula - Server](https://www.bacula.org/) - Bacula is a set of Open Source, computer programs that permit you to manage backup, recovery, and verification of computer data across a network of computers of different kinds. This is for the server installation.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/sysutils/bacula9-server/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/sysutils/bacula) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/sysutils/bacula)

- [![Open-Source Software][OSS Icon]](https://github.com/borgbackup/borg) [BorgBackup](https://borgbackup.readthedocs.io/en/stable/) - BorgBackup (short: Borg) is a deduplicating backup program. Optionally, it supports compression and authenticated encryption. The main goal of Borg is to provide an efficient and secure way to backup data. The data deduplication technique used makes Borg suitable for daily backups since only changes are stored. The authenticated encryption technique makes it suitable for backups to not fully trusted targets.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/archivers/py-borgbackup/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/sysutils/py-borgbackup) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/sysutils/py-borgbackup) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/sysutils/borgbackup) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://github.com/backuppc/backuppc) [BackupPC](https://backuppc.github.io/backuppc/) - BackupPC is a high-performance, enterprise-grade system for backing up Linux, Windows and macOS PCs and laptops to a server's disk. BackupPC is highly configurable and easy to install and maintain.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/sysutils/backuppc/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/sysutils/backuppc) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/sysutils/backuppc) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/sysutils/backuppc) ![](img/termprog.png)

### Desktop Environments

- [![Open-Source Software][OSS Icon]](https://gitlab.gnome.org/GNOME/gnome-shell) [Gnome 3](https://www.gnome.org/gnome-3/) - GNOME 3 provides a focused working environment that helps you to get things done, and it is packed with features that will make you more productive. A powerful search feature lets you access all your work from one place. Side-by-side windows makes it easy to view several documents at the same time.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/x11/lumina/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/wip/lumina) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/wip/lumina) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/x11/lumina)

- [![Open-Source Software][OSS Icon]](https://github.com/KDE) [KDE](https://kde.org/) - K Desktop Environment (KDE) is an Open Source graphical desktop environment for UNIX workstations. Initially called the Kool Desktop Environment it includes a file manager, a window manager, a help system, a configuration system, tools and utilities, and several applications.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/x11/kde5/) [![Available in NetBSD](img/netbsdico.png)](https://ftp.netbsd.org/pub/pkgsrc/current/pkgsrc/x11/kde-workspace4/README.html) [![Available in DragonflyBSD](img/dragonflybsdico.png)](ftp://muug.ca/mirror/dragonflybsd/dports/dragonfly%3A5.10%3Ax86%3A64/LATEST/All/kde5-5.19.5.20.08.1.txz) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/x11/kde)

- [![Open-Source Software][OSS Icon]](https://github.com/lumina-desktop/lumina) [Lumina](https://lumina-desktop.org/) - The Lumina desktop is designed to be fast, customizable, flexible, and lightweight. Lumina works great in multi-monitor configurations and with high-resolution monitors as well as single-screen configurations on laptops or tablets.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/x11/lumina/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/wip/lumina) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/wip/lumina) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/x11/lumina)

## Editors

- [![Open-Source Software][OSS Icon]](https://github.com/mawww/kakoune) [Kakoune](http://kakoune.org/) - Modal editor · Faster as in less keystrokes · Multiple selections · Orthogonal design

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/editors/kakoune/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/editors/kakoune) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/editors/kakoune) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/editors/kakoune) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://github.com/neovim/neovim) [Neovim](https://neovim.io/) - Neovim is an aggressive refactor of editors/vim. It represents a including sensible defaults, a built-in terminal emulator, asynchronous plugin architecture, and powerful APIs designed for speed and extensibility. It retains full compatibility with almost all Vim plugins and scripts. Open the software with `nvim`, not `neovim`.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/editors/neovim/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/wip/neovim) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/wip/neovim) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/editors/neovim) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://github.com/vim/vim) [Vim](https://www.vim.org/) - Vim is a highly configurable text editor built to make creating and changing any kind of text very efficient. It is included as "vi" with most UNIX systems and with Apple OS X.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/editors/vim/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/editors/vim) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/editors/vim) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/editors/vim) ![](img/termprog.png)



### Emulators

- [![Open-Source Software][OSS Icon]](https://www.dosbox.com/wiki/SVN_Builds) [Dosbox](https://www.dosbox.com/) - DOSBox is a DOS-emulator that uses the SDL-library which makes DOSBox very easy to port to different platforms. DOSBox has already been ported to many different platforms, such as Windows, BeOS, Linux, and MacOS.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/emulators/dosbox/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/emulators/dosbox) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/emulators/dosbox) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/emulators/dosbox) ![](img/termprog.png)

### File Managers

- [![Open-Source Software][OSS Icon]](https://github.com/jarun/nnn) [nnn](https://github.com/jarun/nnn) - nnn is a fast and resource-sensitive file browser which integrates well with your DE and favorite GUI utilities, works with the desktop opener, supports bookmarks, has smart navigation shortcuts, has navigate-as-you-type mode, disk usage analyzer mode, comprehensive file details and much more.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/misc/nnn/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/sysutils/nnn) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/sysutils/nnn) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/sysutils/nnn) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://github.com/ranger/ranger) [ranger](https://ranger.github.io/) - ranger is a file manager with VI key bindings. It provides a minimalistic yet nice curses interface with a view on the directory hierarchy. The secondary task of ranger is to psychically guess which program you want to use for opening particular files.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/sysutils/py-ranger/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/wip/py-ranger) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/wip/py-ranger) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/sysutils/ranger) ![](img/termprog.png)

### Network tools

- [![Open-Source Software][OSS Icon]](https://github.com/fish-shell/fish-shell) [Mosh](https://fishshell.com/) - Mosh is a shell designed to withstand intermittant connectivity between two terminals, functioning similarly to ssh

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/net/mosh/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/net/mosh) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/net/mosh) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/net/mosh)  ![](img/termprog.png)

### Office

- [![Open-Source Software][OSS Icon]](https://github.com/KDE/calligra) [Calligra](https://calligra.org/) - Calligra Suite is an office and graphic art suite by KDE. It is available for desktop PCs, tablet computers, and smartphones. It contains applications for word processing, spreadsheets, presentation, vector graphics, and editing databases.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/editors/calligra/) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/editors/calligra)

- [![Open-Source Software][OSS Icon]](https://gerrit.libreoffice.org/) [Libreoffice](https://www.libreoffice.org/) - LibreOffice is a free and powerful office suite, and a successor to OpenOffice .org (commonly known as OpenOffice). Its clean interface and feature-rich tools help you unleash your creativity and enhance your productivity.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/arabic/libreoffice/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/misc/libreoffice) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/misc/libreoffice) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/editors/libreoffice)

### Security

- [![Open-Source Software][OSS Icon]](https://github.com/BastilleBSD/bastille) [Bastille](https://bastillebsd.org/) - Bastille is an open-source system for automating deployment and management of containerized applications on FreeBSD.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/sysutils/bastille/) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://cvsweb.openbsd.org/cgi-bin/cvsweb/src/usr.bin/doas/) [Doas](https://cvsweb.openbsd.org/cgi-bin/cvsweb/src/usr.bin/doas/) - Native to OpenBSD, Doas is a program that replaces the functionality of sudo, allowing a user to do actions as the root user without logging in as the root user. It has a very simple configuration file and multiple modes.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/security/doas/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/security/doas) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/security/doas) ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](https://github.com/fail2ban/fail2ban) [Fail2ban](https://www.fail2ban.org/wiki/index.php/Main_Page) - Fail2Ban scans log files like /var/log/auth.log and bans IP addresses conducting too many failed login attempts. It does this by updating system firewall rules to reject new connections from those IP addresses, for a configurable amount of time. Fail2Ban comes out-of-the-box ready to read many standard log files, such as those for sshd and Apache, and is easily configured to read any log file of your choosing, for any error you wish.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/security/py-fail2ban/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/security/fail2ban) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/security/fail2ban) ![](img/termprog.png)

### Terminal Emulators

- [![Open-Source Software][OSS Icon]](https://github.com/alacritty/alacritty) [Alacritty](https://github.com/alacritty/alacritty) - Alacritty is the fastest terminal emulator in existence. Using the GPU for rendering enables optimizations that simply aren't possible without it. Alacritty currently supports macOS, Linux, BSD, and Windows.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/x11/alacritty/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/x11/alacritty) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/x11/alacritty)

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

- [![Open-Source Software][OSS Icon]](https://github.com/tcsh-org/tcsh) [tcsh](https://www.tcsh.org/) - tcsh is the continuation and successor to csh and expands on its functionalities and capabilities. It is the default root shell on FreeBSD though not its default user shell, and can be installed on the other major BSD's.

   ![Available in FreeBSD](img/freebsdico.png) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/tcsh) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/tcsh) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/tcsh)  ![](img/termprog.png)

- [![Open-Source Software][OSS Icon]](http://zsh.sourceforge.net/Arc/source.html) [Zsh](http://zsh.sourceforge.net/) - Zsh is an extension of the Bourne Shell (bsh) and includes many improvements such as autocorrect, autocompletion, and is extensible with a great deal of many features. Theming is very popular with Zsh. It is the Default Shell on MacOS.

  [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/zsh/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/zsh) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/zsh) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/zsh) ![](img/termprog.png)

  - [![Open-Source Software][OSS Icon]](https://github.com/ohmyzsh/ohmyzsh/) [Oh-My-Zsh](https://ohmyz.sh/) - Oh My Zsh is an open source, community-driven framework for managing your zsh configuration and themes. Can be installed via git or shellscript if not in Ports. The original oh-my-framework.

    [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/ohmyzsh/) ![](img/termprog.png)
<br/>

### Utilities

- [![Open-Source Software][OSS Icon]](https://github.com/bleachbit/bleachbit) [Bleachbit](https://www.bleachbit.org/) - Zsh is an extension of the Bourne Shell (bsh) and includes many improvements such as autocorrect, autocompletion, and is extensible with a great deal of many features. Theming is very popular with Zsh. It is the Default Shell on MacOS.

  [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/wip/bleachbit) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/wip/bleachbit)

***********

## Projects

*Links here are some projects that use the BSD OS in some capacity, Firewalls, Webservers, Gameservers, you name it! Just to give you an idea of what you can do with the OS!*

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
- [Awesome OpenBSD](https://github.com/ligurio/awesome-openbsd) - A List of resources related to the Open BSD Operating System.
- [Awesome UNIX](https://github.com/sirredbeard/Awesome-UNIX) - covers the variety of UNIX likes and has a section for BSD.

***********

## Attribution
*The usage of the BSD Family Tree in the What is BSD FAQ is used under the GNU Free Documentation License Version 1.2 or later. All logos of the various BSD's are the property of their respective projects.*

- FreeBSD® is a registered trademark of The FreeBSD Foundation. in the United States and/or other countries.
- NetBSD® is a registered trademark of The NetBSD Foundation, Inc. in the United States and/or other countries.
- OpenBSD ® is a registered trademark of The OpenBSD Foundation, Inc. in the United States and/or other countries.

***********

## Miscallaneous Web Sources

-[Pkgs.org](https://pkgs.org/) - Pkgs.org is a website dedicated to tracking packages for multiple OS's and also does so for the NetBSD and Free BSD Projects.
-[Why-OpenBSD.Rocks](https://why-openbsd.rocks/fact/) - A site dedicated to various

[UNIX tree]: https://upload.wikimedia.org/wikipedia/commons/7/77/Unix_history-simple.svg
[OSS Icon]: https://svgshare.com/i/R6P.svg
[Money Icon]: https://svgshare.com/i/R6N.svg
