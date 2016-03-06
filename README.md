# git-profile
Manages multiple git configurations as profiles.

```
 $ git-profile 
 
Usage: /Users/dgosselin/bin/git-profile [-c|-r|-s|-v] <config-name>

  Manages multiple Git configurations.

    -c    Creates a new configuration <config-name>, a copy of the current one
    -r    Remove an existing configuration <config-name>, if it exists
    -s    Switch to an existing configuration <config-name>
    -v    View all configurations

```

Create a new git config profile using the profile that you have in place, and set the
new one as the active, marking it with an asterisk.

```
 $ git-profile -c personal
 * personal
   work
```

View all existing git config profiles.

```
 $ git-profile -v
 * personal
   work
```

Switch between multiple git config profiles.

```
 $ git-profile -s work
   personal
 * work
```

When you've got some free time for side projects, switch back to your personal profile.

```
 $ git-profile -s personal
 * personal
   work
```

