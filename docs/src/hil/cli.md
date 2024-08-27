# orb-hil cli

There is a CLI tool to facilitate hardware-in-loop operations. This tool lives
[in the orb-software repo][hil code] and releases can be downloaded
[here](hil-releases). 

It is a single, statically linked CLI tool with lots of features helpful for
development:

* Rebooting orbs into either normal or recovery mode
* Flashing orbs (including downloading from S3, extraction, etc)
* Executing commands over serial
* Automating the login process over serial

## Required peripherals

Different `orb-hil` subcommands require different hardware peripherals. We strongly
recommend at least getting an x86 linux machine and a serial adapter.

Here are the different hardware peripherals necessary for the different subcommands
of `orb-hil`:

* `orb-hil flash`: Needs an x86 linux machine
* `orb-hil reboot`: Needs the serial adapter. See [Hardware Setup][setup]

[setup]: ./hardware-setup.md
[hil code]: https://github.com/worldcoin/orb-software/tree/main/hil
[hil releases]: https://github.com/worldcoin/orb-software/releases?q=hil&expanded=true