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
- [Ports and Programs](#Ports-and-Programs)
    - [Audio](#Audio)
- [Projects](#Projects)
- [How-To's](#How-To's)


## FAQ

##### What is BSD?

![Awesome][UNIX tree]

BSD was originally a UNIX based operating system that was developed at the the University of Berkeley in California in the late 70's. At the time it was a closed source, or partially closed source operating system that was gradually re-engineered into a completely Open source Operating System now used all over the world.

##### How is BSD different than Linux?

BSD takes a more centralized approach in its development having entire program and kernel ecosystems developed together. Whereas Linux itself is just a kernel which then requires groups of people to add packages and other system components together to build the whole operating system, this creates a Linux "Distribution" a distribution of software components (programs, Kernel, drivers and whatnot.)

Because of this difference and because BSD is built around an entire ecosystem from the start, it has an excellent history of documentation for its various functions, both in the Kernel, and with its programs.

For the average UNIX user, it will seem very familiar in many ways, and learning BSD from Linux or other UNIX based Operating Systems will be fairly straightforward, with nearly all of the most common UNIX friendly tools and shells are available for the user.

##### What are the differences between Packages and Ports?

A **Package** (Referred to as a program in this list) is a program already compiled into a binary that can be run on the largest number of systems due to be pre-compiled for you with the most general settings. It requires only the briefest installation, and does not require compilation to run on your machine.

A **Port** is source code with instructions that allow you to compile the code on your machine to create an executable program. It has the advantage of allowing you to compile the program in a more specific way for your machine to get extra performance from the code or only get parts of the program that you need such as only getting the webhost part of an Apache webserver, but no WebDAV or support for User Directories making the program smaller and leaner.

BSD allows installation of both types of software to allow for either ease or flexibility in your OS and environment, it is up to you to decide which you would prefer to use.

##### Can I mix and Match Ports and Packages?

If you know what you are doing, there should be little issue, Issues come when you don't know.

A basic scenario would be this: say you would like to install only part of a webserver, and you modify the port make file to ensure you only install that part. It will function normally, but if you install a program that requires that as a dependency, it may see it, but malfunction due to not having the entirely of that program installed. If the software have no relation to each other, there should be no issues. But when in doubt, install either only ports, or only Packages.

***********

## Ports and Programs

### Audio

- [![Open-Source Software][OSS Icon]](https://github.com/audacity/audacity) [Audacity](http://www.audacityteam.org/) - Free, open source, cross-platform software for recording and editing sounds.
 [![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/audio/audacity/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/audio/audacity) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/audio/audacity) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/audio/audacity)

***********

## Projects

***********

## How-To's




[UNIX tree]: https://upload.wikimedia.org/wikipedia/commons/7/77/Unix_history-simple.svg
[OSS Icon]: https://svgshare.com/i/R6P.svg
[Money Icon]: https://svgshare.com/i/R6N.svg
