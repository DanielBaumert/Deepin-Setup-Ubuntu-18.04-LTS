# Deepin-Setup-Ubuntu-18.04-LTS
Init file explorer and terminal as default

## Install ppa
```bash
sudo add-apt-repository ppa:leaeasy/dde
sudo apt full-upgrade
```
## Install deepin tools
- File explorer
  ```bash
  sudo apt install dde-file-manager
  ```
- Terminal
  ```bash
  sudo apt install deepin-terminal
  ``` 
## Replace file explorer
```bash
sudo xdg-mime default dde-file-manager.desktop inode/directory application/x-gnome-saved-search
```
## Replace terminal
```bash
sudo gsettings set org.gnome.desktop.default-applications.terminal exec 'deepin-terminal'
```
## Clean up 
```bash
sudo apt autoremove
```
# Helpfull feature
## set time by terminal
```bash
sudo cp /usr/share/zoneinfo/Europe/[city] /etc/localtime 
```
