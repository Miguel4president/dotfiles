# Manual Essentials

 * Chrome
 * Iterm2
 * Slack
 * Spectacle
 * f.lux
 * Spotify
 * 1Password
 * Setup iterm + zsh

 The brewfile should get zsh and I might still need to DL oh-my-zsh
 Then make a symlink to the the local zshrc
  * `ln -s $PWD/zshrc_dot_me ~/.zshrc`

That zshrc expects the env.sh file, which is were the bulk of the settings are


## Installed via scripts

* Dash
* Visual Studio Code
  * Plugins for elixir / elm / etc
* Everything in homebrew
* Docker
* asdf
  * All langs through here




# What to do

The install scripts are pretty straight forward
They download stuff, either unzip it into Applications, or mount and copy

Brew will do its thing

If you don't use the 'install-it-all.sh' script then follow these steps most likely


1. Setup the manual stuff, especially zsh and iterm (a little annoying, work in progress)
2. `cd $dotfiles`
3. `sh install/dash`
6. Visual Studio Setup



## Visual Studio Code setup (1 min ideally)

This is unfortunately a little involved still

The install script will do the default install and open it. Then we need to add the `code` command to the PATH, then just rerun the script.

 * `sh vs-code/install`
 * In vs code, open the command pallet 'cmd + shift + p'
  * Search for install shell
 * Open a new terminal
 * `which code`
  * should spit out /usr/local/bin/code
 * `sh vs-code/install`

# Keeping me up to date

To keep this stuff up to date run the `update-settings.sh` script

It dumps
 * Current brew status
 * VS code settings
 * VS code packages
