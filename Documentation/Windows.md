NodeJS Windows Installation
===========================

## Installation Instructions

From an a Powershell context with Adminstrator privileges, use
[Chocolatey](https://chocolatey.org) to install `nodejs`.

~~~~~~powershell
PS \> choco install nodejs
~~~~~~

### Check Installation

Use the `--version` switch to verify the `node` and `npm` binaries have been
installed; any version is fine, as long as no error occurs when the command is
run.

~~~~~~powershell
PS \> node --version
v7.9.0

PS \> npm --version
4.2.0
~~~~~~
