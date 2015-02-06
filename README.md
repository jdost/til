# TIL

A collection of shell scripts to aid the collecting of information from your day to 
day work.

## Command

Everything runs through the `til` command.  It wraps a series of simple scripts to
handle organization and traversing the various bits of information you want to 
record.  These include:

* `diary` - Creates a file for the current day to help log information from 
  throughout the day, e.g. `til diary`
* `project` - Takes an argument for the project to edit/create, opens a file to help
  record thoughts on a project, e.g. `til project til`
* `topic` - Takes a hierarchical name for a subject/topic to edit some information
  on, e.g. `til topic zsh/completions`
* `browse` - Opens vim as a filebrowser of the current files in the repository
* `grep` - Searches through the repository for the pattern, e.g. `til grep TODO`
* `tag` - Lists files that contain the given tag, tags are denoted with a `+`
* `commit` - Commits the current state to a git repository

## Setup

The TIL repository will be setup in the current directory if no environment variable
`$TILHOME` is set, otherwise it will use that location to write to.
