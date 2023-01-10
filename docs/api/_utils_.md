---
tilte: lsd module _utils_
description: lsd module _utils_ description
---


# lsd module _utils_

This script defines several utility functions for tasks such as listing and deleting files, managing processes, and manipulating images.

* `lsd-mod.utils.pid` takes a process name as an argument and outputs the process IDs of any processes with a command line that matches the given process name.

* `lsd-mod.utils.alpha-numeric` takes a string as an argument and outputs only the alpha-numeric characters in the string.

* `lsd-mod.utils.kill` takes a process name as an argument and kills all processes with a command line that matches the given process name.

* `lsd-mod.utils.kill.python` is a convenience function that calls lsd-mod.utils.kill with python as the process name argument, effectively killing all Python processes.

* `lsd-mod.utils.ls` lists the files in the current directory, including their permissions in octal notation.

* `lsd-mod.utils.ls.pycache` and `lsd-mod.utils.ls.egg` functions list the __pycache__ and .egg-info directories in the current directory, respectively, including their permissions.

* `lsd-mod.utils.rm.pycache`, `lsd-mod.utils.rm.egg`, and `lsd-mod.utils.rm.node_modules` functions delete the __pycache__, .egg-info, and node_modules directories respectively in the current directory.

* `lsd-mod.utils.trash` takes a list of file names as arguments and moves them to the user's trash directory.

* `lsd-mod.utils.image.resize` takes a file extension and a percentage as arguments and resizes all files with the given extension in the current directory by the given percentage.

* `lsd-mod.utils.image.pdf` takes a file extension as an argument and converts all files with the given extension in the current directory into a single PDF file.

* `lsd-mod.utils.date.get` outputs the current date in the format "DD-Mon-YYYY, DayOfWeek".

* `lsd-mod.utils.system.info` outputs system information using the inxi command.

* `lsd-mod.utils.id.salt` outputs a randomly generated security key or salt string.