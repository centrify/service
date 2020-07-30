# DISCLAIMER

This fork of kardianos/service is temporary and is intended for Centrify's internal use.
It is not supported or maintained by Centrify. 
Please refer to the original location https://github.com/kardianos/service for latest versions of the module.

# service [![GoDoc](https://godoc.org/github.com/kardianos/service?status.svg)](https://godoc.org/github.com/kardianos/service)

service will install / un-install, start / stop, and run a program as a service (daemon).
Currently supports Windows XP+, Linux/(systemd | Upstart | SysV), and OSX/Launchd.

Windows controls services by setting up callbacks that is non-trivial. This
is very different then other systems. This package provides the same API
despite the substantial differences.
It also can be used to detect how a program is called, from an interactive
terminal or from a service manager.

## BUGS
 * Dependencies field is not implemented for Linux systems and Launchd.
 * OS X when running as a UserService Interactive will not be accurate.
