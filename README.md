# Swift CLI Cheatsheet

A list of the swift CLI application commands. 

CLI commands

| Command | Description |
|---------|-------------|
| swift -version | Output the current version of the Swift CLI |
| swift -help  | list the CLI help |

CLI Subcommands (Swift Package Manager)

| Command | Description |
|---------|-------------|
| swift package | perform operations on Swift packages |
| swift build | build source in binary |
| swift run | build and run an executable product |
| swift test | build and run tests |
| swift help <subcommand> | list the help for the supplied subcommand |

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

Package Dependencies
  
| Command | Description |
|---------|-------------|
| swift package resolve | Resolve package dependencies |  
  
Build Options

| Command | Description |
|---------|-------------|
| swift build --target  | build using the supplied target configuration (target as stored on the Package .swift file |
| swift build --product | build using the supplied product configuration (produce as stored on the Package .swift file |

Running Unit Tests

| Command | Description |
|---------|-------------|
| swift test | runs all unit tests |
| swift test --filter MyTestName | runs tests using the supplied filter or just supply the name of the test to run just that one |
| swift test -l | list test methods |
  
REPL Commands

| Command | Description |
|---------|-------------|
| swift   | lauches the swift REPL |
| :quit   | quit/exit the REPL |
| :help   | list the REPL help |
