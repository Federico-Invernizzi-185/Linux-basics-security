# Sudo and SUID – Linux Privilege Escalation Basics

## What is sudo

Sudo allows a permitted user to execute a command as the root user
or another user, according to system configuration.

It is commonly used by system administrators to perform tasks that
require elevated privileges while maintaining user accountability.

## What is root

The root user is the superuser in Linux systems.
It has unrestricted access to the entire system and can read, modify
or delete any file and configuration.

For security reasons, direct access to the root account is usually
restricted, and administrative tasks are performed using Sudo.

## What is SUID

SUID (Set User ID) is a special permission that allows a file to be
executed with the privileges of its owner, instead of the user who
launched it.

## Security implications

SUID binaries represent a potential security risk if they are
misconfigured or contain vulnerabilities.

If an attacker is able to exploit a SUID program owned by root,
they may gain elevated privileges and compromise the entire system.

For this reason, SUID permissions must be carefully audited
and limited to trusted system binaries only.

## Practical example

The presence of the SUID bit can be identified using the 'ls -l' command.

Example:
-rwsr-xr-x

In this case, the 's' in the owner execute position indicates that
the binary will run with the privileges of its owner.

System administrators should regularly check for unexpected SUID
binaries and remove the permission when not strictly required.


When SUID is set on a binary owned by root, the program runs with
root privileges, even if executed by a normal user.
