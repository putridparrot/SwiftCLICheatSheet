# Swift CLI CheatSheet

A list of the swift CLI application commands. 

REPL Commands

| Command | Description |
|---------|-------------|
| swift   | lauches the swift REPL |
| :quit   | quit/exit the REPL |
| :help   | list the REPL help |

CLI commands

| Command | Description |
|---------|-------------|
| swift -version | Output the current version of the Swift CLI |
| swift -help  | list the CLI help |
| swift help    | list the CLI help |

CLI Subcommands (Swift Package Manager)

_Note: you can use swift help subcommand to get help on a given subcommand._

| Command | Description |
|---------|-------------|
| swift help  | list the CLI help |
| swift package | perform operations on Swift packages |
| swift build | build source in binary |
| swift run | build and run an executable product |
| swift test | build and run tests |

Package Options

_Run these commands from the folder where you want your package written to_

| Command | Description |
|---------|-------------|
| swift package init | Create a library package (default) |
| swift package init --type empty | Create an empty package |
| swift package init --type library | Create a library package |
| swift package init --type executable | Create an executable package |
| swift package init --type system-module | Create a system module package |
| swift package init --type manifest | Create a manifest package |

Add --name to the _package_ subcommand to supply a package name, for example

| Command | Description |
|---------|-------------|
| swift package init --name MyPackageName | Create a library package (default) with supplied name |

Build Options

| Command | Description |
|---------|-------------|
| swift build --target  | build using the supplied target configuration (target as stored on the Package .swift file |
| swift build --product | build using the supplied product configuration (produce as stored on the Package .swift file |
