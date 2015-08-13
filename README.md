# Utility Belt
Useful tools for the day to day life of a developer. Utility Belt provides a set
of useful tools to manage your development work flow. All tools must be made
executable using `chmod +x tool-name`. All executables within this repo will be
linked to $HOME/.bin when you run the install script.

# Requirements
- `ruby > 2.0`
- `bundler > 1.0.0`
- `ruby gems > 2.0`

# Installation
Add this to your bashrc/zshrc or other init files:
```
export PATH="$PATH:$HOME/.bin"
```
This will makes sure that all the executables stored in .bin folder can be discovered and run on the command line. Then you should run the install script to symlink the right executables
```
$ git clone https://github.com/hackers-of-umass/utility-belt.git
$ cd /path/to/utility-belt && bundle install
$ ./install
```

# Purpose
Why not just use gems or pip or brew to manage your cmd line tools you ask? The purpose to utility belt is to provide a set of "micro" tools for your own personal usage outside of more heavy weight tools.

# Contributing
To add a new tool to Utility Belt, simply create an executable in a folder that best represents the function of the tool. Each tool must be self contained with enough helpful hints on how to use them. Tools written in Ruby and Shell are preferred.

You MUST make your tools executable by running `chmod +x tool-name`
