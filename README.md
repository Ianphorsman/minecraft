Overview
--------

This is a deployment and console wrapper for Minecraft which allows for more
convenient administration of a Minecraft server.

Installation
------------

    gem install minecraft

This will install the Minecraft extension library and binary, the Minecraft
server jarfile will be downloaded from http://minecraft.net when the binary is
ran for the first time.

Usage
-----

    mkdir ~/MinecraftServer
    cd ~/MinecraftServer
    minecraft

    minecraft -h

Current Features
----------------

Please refer to `Minecraft::Extensions#initialize`.

    !give <item> <quantity>       # Gives the user an <item>, the <quantity> 
                                  # upper bound is 2560 unlike the Minecraft 
                                  # default of 64.  Items can be specified by
                                  # approximate name.
    !giveall <item> <quantity>    # Gives all connected users an <item>.
    !tp <target_user>             # Teleports the user to the <target_user>.
    !tpall                        # Teleports all connected user to the user.
    !nom                          # Give a golden apple the user.
    !nomall                       # Give a golden apple to every connected user.
    !kit <group>                  # Gives a kit to the user.
    !kitall <group>               # Give a kit to every connected user.
    !kitlist                      # Lists the available kits.
    !addtimer <item> <frequency>  # Adds a timer to give <item> to the user ever <frequency> seconds.
    !deltimer <item>              # Delete a timer associated with <item>.
    !printtimer                   # Print timers of the user.
    !printtime                    # Print the current counter time.
    !list                         # List the connected users, notes ops.
    !property                     # Check a server property (!property spawn-monsters).
    !s <label> <command>          # Associates a command to a shortcut label for the user.
    !s <label>                    # Runs the command with the associated label.
    !shortcuts                    # Lists the users shortcuts.
    !rules                        # Prints the server rules.
    !uptime <user>                # Prints the uptime of the given user.
    !uptime                       # Prints the uptime of the current user.
    !help                         # Outputs the help contents.

Development Path
----------------

### Minor Release Milestone

- Automated tests written
- Documentation
- Thorough testing

### Major Release Milestone

- Complete test coverage
- Complete documentation coverage
- All feature requests closed
- All bugs closed
- Thorough testing done across multiple environments


### Semantic Versioning

- http://semver.org
- Currently patch level releases are being made, nothing is stable yet.
- Once tests and documentation has been written a stable minor release will be
committed.
- Once the repository is completely stable and I am satisified with the feature
set, a major version will be released.  Any chances afterwards are backwards
compatible until the major version is incremented.

Contributors
------------

Forks are welcomed, pull requests will be prompty reviewed!

- Ian Horsman

Notice
------

Minecraft is copyright of Mojang AB and developed by Markus Persson (@notch).
