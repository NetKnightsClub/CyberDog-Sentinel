# CyberDog Sentinel – Master Controller 

Welcome to **CyberDog Sentinel**! 🐾 A highly unhinged but surprisingly effective set of scripts designed to keep watch over your home network, scan for devices, and keep things in check with the occasional rogue device removal (because why not?). All powered by **Python** and **bash**. A must-have for your home network security *if* you're into the whole chaotic-but-functional approach to cybersecurity. 

## Features 🚀

- **Network Scanner**: Scans your local network and identifies devices via `nmap`.  
- **Port Watcher**: Monitors open ports on your system and logs the activity.  
- **Device Logger**: Keeps an eye on the devices connected to your network by logging ARP tables.  
- **Rogue Device Kicker**: Automatically checks for rogue devices and blocks them based on their MAC address. (Because who doesn’t love kicking out unwanted guests?)  
- **Log Everything**: All activity is logged in handy logs so you can sit back and monitor the chaos.

## Requirements 📦

Before using **CyberDog Sentinel**, make sure you have the following installed:

- `Python 3.x`
- `nmap` (for network scanning)
- `ss` (for port monitoring)
- `arp` (for device logging)
- `arptables` (for rogue device blocking)

## Setup 🚧

1. Clone the repo:
   
`git clone https://github.com/VisAwesme/CyberDog.git`

3. Install dependencies:

- `sudo apt install nmap iproute2 net-tools` (Ubuntu/Debian/Parrot Security OS/BackBox/DEFT Linux/CAINE/Kali Linux package manager)
- `sudo pacman -S nmap iproute2 net-tools` (Arch/ArchStrike/BlackArch Linux package manager)

3. Run the master controller:

   ` python3 cyberdog_sentinel.py`

## Usage ⚙️

 - CyberDog Sentinel will start running and periodically scan your network for devices, watch open ports, and log connected devices.

 - If any unauthorized device is detected, it will be blocked from the network.

 - Logs are (hopefully) saved in the logs/ directory for review.

## License 📝

This project is licensed under the [MIT](https://github.com/VisAwesme/CyberDog/blob/main/LICENSE) License. See LICENSE for more information.

Made with love (and a bit of chaos) by Kel 🖤

"Because you shouldn't trust that one guy who uses Windows." 💀
