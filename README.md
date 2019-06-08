## find_path [![HitCount](http://hits.dwyl.io/GiovaLomba/wd.svg?style=plastic)](http://hits.dwyl.io/GiovaLomba/find_content)

It looks for items into the target location whose pathname matches the
given pattern. The name `find_path` has been chosen keeping account of
the comprise between having a meaningful name and typing laziness.

#### Why YAST (Yet Another Search Tool)?

Looking for files is easy, really less when you have a lot of them (as
we all usually do). Personally I've not very clear all assumptions and
configuration the modern operating systems and their shipped utilities
apply during search. So, to be in control, here are some reason:

+ **Flexibility**: I can search for pattern in paths maybe using regex.
+ **Filtering**: Metadata filtering, creation, access, edit, file size,
  ecc.
+ **Control**: Knowing exactly what is happening controlling verbosity.
+ **Multiprocessing**: You can feel a bit like the gladiator when: *At
  my signal, unleash hell!*
+ **BS 1**: I wanted to revamp and improve a more than five year old
  search software.
+ **BS 2**: I could do it, so I did it.

#### Reasonable defaults?

The following is a list (not necessarily exhaustive) of settings the 
software application implements as defaults behaviours:

- By default it uses `1` single process in a sequential fashion [ this
  because in most of the cases `1` process performs significantly better
  than more than one does].
 
 You knows: *good fences make good neighbours!*
 
#### How does it works?

Here you can learn about the features the `find_path` application
exposes to the users, how and when should they be used.

```
(c) 2019 Giovanni Lombardo mailto://g.lombardo@protonmail.com
find_path version 1.0.0

usage: whereis.py [-h] [-bf [BEFORE]] [-af [AFTER]] [-ac] [-ae] [-aa]
                  [-p [PROC]] [-v]
                  location pattern

It looks for files into the target location whose names matches the given pattern.

defaults behaviours:
 - Single process.

positional arguments:
  location              The location to look for matching items.
  pattern               The pattern to look for into items content.

optional arguments:
  -h, --help            show this help message and exit
  -bf [BEFORE], --before [BEFORE]
                        The 'before' reference date in the format %Y-%m-%d %H:%M
  -af [AFTER], --after [AFTER]
                        The 'after' reference date in the format %Y-%m-%d %H:%M
  -ac, --created        When given it evaluates the created attribute of selected files.
  -ae, --edited         When given it evaluates edit attribute of selected files.
  -aa, --accessed       When given it evaluates last access attribute of selected files.
  -p [PROC], --processes [PROC]
                        The number of processes to start for the task.
  -v, --verbose         Logs verbose output (really slow).
  
Elapsed time 'find_path':  0.000997 seconds.
```

#### Contributions [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=plastic)](https://github.com/GiovaLomba/find_content/issues)

Contributions are always welcomed. Here a reasonably short list of
things you can contribute with:

+ You find a misbehaviour (aka bug): please report the issue so that it
can be fixed and all can benefits of the fix.

+ The software has been tested only on the OS versions mentioned below:
if you use the software on other platforms and it works, please report
the fact so that the documentation can be updated.

+ You would like the application to be able to do something it does not:
please request the features, it may be even quick and easy to implement.

+ You can write tutorial on specific or uninteded usages of the software.

+ You can enrich the documentation with real usage examples and use cases.

#### Download

+  [Windows 10 amd64](https://github.com/GiovaLomba/find_path/raw/master/find_path.exe)
   -  **MD5** |8ecb2ab5f7f845dbce415163b53e129a|
   -  **SHA256**
      |5b643c8f4d2adae05ba5d874f201aee792c71cb1f85a756daa3bb26d0e426fa4|
   -  **VirusTotal**
      |[VirusTotal](https://www.virustotal.com/gui/file/5b643c8f4d2adae05ba5d874f201aee792c71cb1f85a756daa3bb26d0e426fa4/detection)|
      
#### Powered by

![Python](https://www.python.org/static/img/python-logo.png "Python")
<br/> 

<!--
![PyInstaller](https://www.pyinstaller.org/_images/pyinstaller-draft1c-header-trans.png)
-->
