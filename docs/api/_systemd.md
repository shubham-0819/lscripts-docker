---
tilte: lsd module _systemd
description: lsd module _systemd description
---


# lsd module _systemd

This script is a collection of functions for working with the systemd init system in Linux. The functions are all prefixed with lsd-mod.systemd and have different suffixes indicating their specific behavior.

* `lsd-mod.systemd.get__vars()` this function logs the message "systemd-cfg::" to the console.

* `lsd-mod.systemd.list.enabled()` uses the systemctl command to list all systemd services that are enabled.

* `lsd-mod.systemd.list.running()` uses the systemctl command to list all systemd services that are currently running.

* `lsd-mod.systemd.list.active()` uses the systemctl command to list all systemd services that are active, whether they are running or not.

* `lsd-mod.systemd.list.all()` uses the systemctl command to list all systemd services that are installed.

* `lsd-mod.systemd.nvm.create-service-config()` takes one optional parameter and creates a systemd service file with the provided service name, otherwise defaults to basename $PWD.service
It creates a service file by using tee command which is redirecting the content of here-document to the file.

* `lsd-mod.systemd.main()` function is the entry point of the script. It sets up some environment variables, imports the argparse.sh and common.sh scripts, which are used to parse command-line arguments and provide some common utility functions, respectively.
