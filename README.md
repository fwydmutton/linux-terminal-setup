# Linux Terminal Setup

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

## Screenshot/Preview
![image alt](https://github.com/fwydmutton/linux-terminal-setup/blob/b75a7c514ee8539911976cdccb15b82a2db3e85c/Screenshot_20260411_081712-1.png)
![image alt](https://github.com/fwydmutton/linux-terminal-setup/blob/main/Preview/terminal-with-starship-preview2.png?raw=true)

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

# STARSHIP CONFIG
Now lets add more taste to the terminal by adding starship to the terminal.

## Install Starship

Fedora
```
sudo dnf install starship
```
Arch
```
sudo pacman -S starship
```
Debian or Ubuntu
```
curl -sS https://starship.rs/install.sh
 | sh
```
## Enable it in your shell

Bash
```
echo 'eval "$(starship init bash)"' >> ~/.bashrc

source ~/.bashrc
```
Zsh
```
echo 'eval "$(starship init zsh)"' >> ~/.zshrc
source ~/.zshrc
```
Fish
```
echo 'starship init fish | source' >> ~/.config/fish/config.fish
```
## Basic config file

## Create config folder
```
mkdir -p ~/.config
```
## Create config file
```
nano ~/.config/starship.toml
```
The deffault location for the toml file is:

## home/.config/starship.toml

## After creating the config file copy paste the starship.toml from setup files. To customize your Os Choose from the symbols and copy paste at the top. For default I'm using Fedora, so the first symbol under os symbols is Fedora, but you can customize it to your liking.
