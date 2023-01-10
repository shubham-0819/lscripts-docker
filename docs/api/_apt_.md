---
tilte: lsd module _apt_
description: lsd module _apt_ description
---


# lsd module _apt_

This script provides functions for managing packages on a Debian-based system using apt-get. The functions allow users to search for and install packages, add and remove repositories, update and upgrade packages, and perform various cleanup tasks. The functions include lsd-mod.apt.search, lsd-mod.apt.guess, lsd-mod.apt.get-repo, lsd-mod.apt.add-repo, lsd-mod.apt.update, lsd-mod.apt.install, lsd-mod.apt.uninstall, lsd-mod.apt.purge, lsd-mod.apt.clean, and lsd-mod.apt.autoremove.

* `lsd-mod.apt.get__vars` Is currently empty, as indicated by the lsd-mod.log.echo "Nothing here yet!" command.

* `lsd-mod.apt.search` Takes a single search phrase as an argument and searches for available packages in the apt cache that match the given search phrase. The names of the matching packages are then passed to the apt-cache policy command to show the package policy information, and the names of the packages are also output.

* `lsd-mod.apt.guess` Also takes a single search phrase as an argument and searches for available packages in the apt cache that match the given search phrase. It then filters the output to include only the lines that begin with the search phrase and outputs a command to install the packages.

* `lsd-mod.apt.get-repo` Lists the repositories that have been added to the system's apt configuration or removes them, depending on the value of the _type argument. If the _type argument is not provided, it defaults to ls (list).

* `lsd-mod.apt.add-repo` Adds a PPA (Personal Package Archive) repository to the system's apt configuration. It takes a single argument in the form of a PPA repository specification (e.g., ppa:user/ppa-name) and adds it to the system using the apt-add-repository command. The function also creates a backup of the apt configuration in a file with a unique name based on the current system information and time.

* `lsd-mod.apt.update` Updates the package list index and then upgrades all installed packages to their latest versions.

* `lsd-mod.apt.install` Installs one or more packages specified as arguments to the function. If no package names are provided, the function displays an error message.

* `lsd-mod.apt.uninstall` Uninstalls one or more packages specified as arguments to the function. If no package names are provided, the function displays an error message.

* `lsd-mod.apt.purge` Removes one or more installed packages and their configuration files, specified as arguments to the function. If no package names are provided, the function displays an error message.

* `lsd-mod.apt.clean` Removes all packages marked for deletion by apt-get. It also removes all downloaded package files that are no longer needed, as well as old package files that can no longer be downloaded.

* `lsd-mod.apt.autoremove` Removes all packages that were installed as dependencies but are no longer required by any installed package. It also removes all packages that are no longer available in the package repositories.