# Linux File Permissions

## Overview
Linux file permissions define who can read, modify or execute a file.
They are a core security mechanism to protect the system from unauthorized access.

## Permissions format
Example output of the `ls -l` command:

-rwxr-xr--

- Owner: read, write, execute
- Group: read, execute
- Others: read only

## Commands used
- ls -l
- chmod
- chown

## Commands explanation

### ls -l
Displays detailed information about files and directories, including permissions, owner, group and size.

### chmod
Changes file permissions, using symbolic or numeric notation.

### chown
Changes the owner and group of a file or directory.

## Numeric permissions (chmod 750)

Linux permissions can also be represented using numbers.

Each number is the sum of:
- read (4)
- write (2)
- execute (1)

## Practical example:
chmod 750 script.sh

Permissions result:
- Owner: 7 (4 + 2 + 1) → read, write, execute
- Group: 5 (4 + 1) → read, execute
- Others: 0 → no permissions

## Security considerations
Incorrect fle permissions can allow unauthorized users to execute or modify files, potentially leading to security risks.
