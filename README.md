# Script doctor examples for Development Kit

Repository starting point issue (in French): https://github.com/stephane-klein/backlog/issues/323

## Why this project?

I use the contents of this repository (["Prerequisites" skeleton](prerequisites-skeleton.md) and [`./scripts/doctor.sh`](`./scripts/doctor.sh)) to write the README "Prerequisites" section of my projects and to implement a script called `doctor.sh` to check that the developer environment is correctly installed and configured.


## How to use this repository?

- Step 1: I copy the ["Prerequisites" skeleton](prerequisites-skeleton.md) file sections that match with the tools I'm using in the project I want to document.
- Step 2: I copy the [`./scripts/doctor.sh`](`./scripts/doctor.sh) file to the project I develop, and I delete useless content.

## Example

See https://github.com/stephane-klein/postgres-playground-skeleton/tree/main

## FAQ

**Q1**. Why not implement a script that installs all the tools automatically?<br />
**R1**. These tools are installed on my personal desktop OS. I use this OS for other purposes than running this project.
I want to control what I install on my OS and how install it. I don't want to run a script that automatically installs everything on my OS, without understand exactly what is installed and how it is installed.

**Q2**. Why don't use Ansible to check installation and install tools?<br />
**R2**. I don't what to install automatically this tools (see **R1**). I think Ansible is overkill compared to a "simple" bash script, which is very "straightforward".

**Q3**. This project tests very few things, very few tools. Is this normal?
**R4**. Yes, that's normal, this is a young project and I'll be adding test scripts and
installation instructions progressively. You can see [here](https://github.com/stephane-klein/development-kit-doctor-scripts/issues)
the list of the next improvements I want to implement.
