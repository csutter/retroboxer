# retroboxer
💾 Easily run 86Box emulated retrocomputing machines

## Disclaimer
This is a pet project and I'm not sure how motivated I am to clean it up or make it general enough
to be used for anyone. This repository may contain hardcoded locations and paths specific to my
setup and use cases, and there is no guarantee that it'll work anywhere else.

That said, it may inspire you to copy and adapt!

## Motivation
I love indulging my nostalgia for late 1990s/early 2000s computing. [86Box][86box] is the most
reliable and accurate macOS-compatible tool I have found for this purpose (other than my collection
of actual period hardware), but can be a bit convoluted to run without a Windows-only configuration
manager.

This repository contains:
- My own minimum viable configuration manager
- 86box template configuration files for several "era appropriate" emulated machines
- Notes on installing and configuring assorted vintage operating systems

## Requirements
- macOS
- Bash (I use a recent upsteam Bash instead of the default macOS one, YMMV)
- 86Box (installed into `/Applications`)
- This repository's `bin` folder on your PATH
- A dedicated directory for storing your machines, e.g. `~/86box` (run `rb-*` commands from that
  directory)

## Usage
> Note: The following assumes you are running commands from your machine storage directory

### Create a new machine from a template
```bash
# Creates a machine called "win95" from the template "1996-pentium133"
$ rb-create 1996-pentium133 win95
```

### Run a virtual machine
```bash
# Runs the machine "win95"
$ rb-run win95
```

[86box]: https://86box.net
