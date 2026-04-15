## Linux Terminal Setup

Simple guide to set up a clean terminal using bash and fastfetch, (Beginner Friendly).

## Features

- Clean bash configuration
- Fastfetch system info on startup
- Custom aliases
- Auto fastfetch on startup
- Audio info and media player info

# Need to download font from [here](https://www.nerdfonts.com/font-downloads) otherwise the icons won't be printed on the terminal. You can choose whichever font you like, but it must be from Nerdfonts.

  ## Files

bash/.bashrc → shell config  
fastfetch/config.jsonc → system info display  

## Screenshot
![image alt](https://github.com/fwydmutton/linux-terminal-setup/blob/b75a7c514ee8539911976cdccb15b82a2db3e85c/Screenshot_20260411_081712-1.png)

## Editing Bashrc
- Run the command
  ```
  nano ~/.bashrc
  ```
  And copy paste the text from Setup Files/basrc
- After editing the bashrc file from setup file. Run the command source

  ```
  ~/.bashrc

- To save the bashrc file's source

## Installing Fastfetch
On Fedora or Nobara:
```
sudo dnf install fastfetch
```
On Ubuntu or Debian:
```
sudo apt install fastfetch
```
On Arch:
```
sudo pacman -S fastfetch
```
Check it works:
```
fastfetch
```
## Create a config file

Run:
```
fastfetch --gen-config
```
This creates:
~/.config/fastfetch/config.jsonc

## Edit the JSON file

Run:
```
nano ~/.config/fastfetch/config.jsonc
```
## Setup and Customization
- Copy paste the text from Setup files/json
- To add a logo, set the logo path, for example /home/yourname/Pictures/logo.png
- Adjust height and width as needed
- Save the file
- Open the terminal to see changes
- Restart the terminal if changes do not appear

And you're good to go!!!
  
