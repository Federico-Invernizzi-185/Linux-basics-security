# Users and Groups in Linux

## Users

Linux is a multi-user operating system, meaning that multiple users
can work on the same system with different levels of access.

Each user is identified by a unique user ID and has specific
permissions that define what they can read, modify or execute.

## Root and standard users

The root user is the system administrator and has full control over
the operating system.

Standard users have limited privileges and are restricted from
performing administrative actions, which helps protect the system
from accidental or malicious changes.

## Groups

Groups are used to manage permissions for multiple users at the same time.

Each file in Linux has an owner and an associated group.
By assigning users to groups, administrators can control access
to files and resources in a structured and scalable way.

## Useful commands

- `whoami` → shows the current user
- `id` → displays UID, GID and group memberships
- `groups` → shows the groups a user belongs to
- `useradd` → creates a new user
- `groupadd` → creates a new group
- `usermod -aG` → adds a user to a group

## Security note

Proper user and group management is essential to system security.

Incorrect group assignments or excessive privileges can allow
unauthorized access to sensitive files or system functions,
violating the principle of least privilege.

## Conclusion

Understanding users and groups is fundamental for managing access
control and maintaining a secure Linux system.
