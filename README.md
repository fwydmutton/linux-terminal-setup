## Linux Terminal Setup

Simple guide to set up a clean terminal using bash and fastfetch.

## Features

- Clean bash configuration
- Fastfetch system info on startup
- Custom aliases
- Auto fastfetch on startup
- Audio info and media player info

  ## Files

bash/.bashrc → shell config  
fastfetch/config.jsonc → system info display  

## Screenshot
![image alt](https://github.com/fwydmutton/linux-terminal-setup/blob/b75a7c514ee8539911976cdccb15b82a2db3e85c/Screenshot_20260411_081712-1.png)

## Editing Bashrc
- After editing the bashrc file from setup file. Run the command source

  ```~/.bashrc
  to save the bashrc file's source

## Installing Fastfetch
On Fedora or Nobara:
sudo dnf install fastfetch

On Ubuntu or Debian:
sudo apt install fastfetch

On Arch:
sudo pacman -S fastfetch

Check it works:
fastfetch

Create a config file

Run:
fastfetch --gen-config

This creates:
~/.config/fastfetch/config.jsonc

Edit the JSON file

Open it:
nano ~/.config/fastfetch/config.jsonc 
Copy paste the text from setup files/json file

And you're good to go!
  
