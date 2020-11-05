## Guidelines to contribute

> Simply put the name of the **application** in the list, and make sure you add ports to the software if some exist. If it's available only in Git, that's no worry.
> Link to its **homepage** or a **guide** on how to install it, ideally you will have installed it so you know the process and know that the program functions correctly.
> Also write a **short description** for the application + add **icon**. (If the program also has a blurb on it's homepage of it's functions that also works.)
> Make sure it is put under the **appropriate topic**. That can always be clarified in the pull request if neccesary.
> Ensure everything is **alphabetically sorted**.

***********

## Unsure how to contribute?

- [How to Use Github](https://guides.github.com/activities/forking/)
- [How to Git from the Command Line](https://rogerdudler.github.io/git-guide/)
- [What is Markdown?](https://github.com/luong-komorebi/Markdown-Tutorial) - Markdown is the writing method used to create this list, if you want to know how to format properly, it's best that you learn how to use Github Markdown.
- [Alternative Markdown Guide:](https://guides.github.com/features/mastering-markdown/)

The format is pretty straightforward:

```- [![Open-Source Software][OSS Icon]](http://OPENSOURCECODE.git.com) [NAME OF PROGRAM](PROGRAM HOMEPAGE) - This is an explanation of what the program does written by you or a copy of the official explanation of the program from the programs homepage. either works fine here.```

  ```[![Available in FreeBSD](img/freebsdico.png)](https://www.freshports.org/shells/zsh/) [![Available in NetBSD](img/netbsdico.png)](https://pkgsrc.se/shells/zsh) [![Available in DragonflyBSD](img/dragonflybsdico.png)](https://pkgsrc.se/shells/zsh) [![Available in OpenBSD](img/openbsdico.png)](https://openports.se/shells/zsh) ![](img/termprog.png)```

This second block is one tab over, to make sure that the icons line up, the links in this block all go to either: Freshports.org, pkgsrc.se, or openports.se. Freshports for FreeBSD, pkgsrc for Dragonfly and NetBSD, and Openports for OpenBSD.  If the BSD in question doesn't have a port available in any one or all of the sites, remove the whole object. Please insert the ![](img/termprog.png) if the program is terminal only to clarify where the program can be used, either on a window manager desktop or command line.
