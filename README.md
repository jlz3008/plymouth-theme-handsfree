# plymouth-theme-install
Script Plymouth theme oriented to develop install sticks without 
user interaction

The target of this theme is create a USB stick with SysLinux and
install software or make maintenance operations without any 
user selection or confirmation.

## Main Idea

Get a "plymouth console" with scroll where show progress messages.
No progress bar is needed.

## Commands

Only *plymouth message* command is used to interact with script.

A simple *plymouth message* command show text on last console line

```bash
  plymouth message --text="Text to log"
```

You can set the title console

```bash
  plymouth message --text="title: The title text"
```

You can hide the console and show a big text

```bash
  plymouth message --text="big: The big text"
```

Or simply hide and show the console

```bash
  plymouth message --text="hide:"
  plymouth message --text="show:"
```

## Configure the script

You can configure the logo, image and position, console text, colors and position, background, 
color or image,  modifiying the script configuration
at the end of script text.

# Example test

There is a complete example on [test]( https://github.com/jlz3008/plymouth-theme-handsfree/blob/master/test) bash script file.

# External links

* Basic Plymouth documentation http://www.freedesktop.org/wiki/Software/Plymouth/Scripts/
* Some Plymouth documentation http://brej.org/blog/?cat=16
* How to test the theme on a Ubuntu Box https://wiki.ubuntu.com/Plymouth
* Last Resource Information http://cgit.freedesktop.org/plymouth
