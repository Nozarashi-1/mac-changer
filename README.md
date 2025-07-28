MAC Address Changer

A simple Python script to change the MAC address of a network interface on Linux-based systems.

📌 Description

This program allows users to spoof the MAC (Media Access Control) address of a specified network interface. MAC spoofing can be useful for testing network security, enhancing privacy, or bypassing MAC filters on networks.

    ⚠️ Note: This script requires root privileges and works only on systems with the ifconfig utility.

🚀 Features

    Get the current MAC address of a given network interface.

    Set a new, user-specified MAC address.

    Verifies if the MAC address change was successful.

🛠️ Requirements

    Python 3.x

    Linux operating system

    ifconfig command-line utility (usually provided by net-tools)

🔧 Installation

Clone the repository:

    git clone https://github.com/your-username/mac-changer.git
    cd mac-changer

⚙️ Usage

Run the script with the required options:

    sudo python mac_changer.py -i <interface> -m <new_mac>

Example:

    sudo python mac_changer.py -i eth0 -m 00:11:22:33:44:55
    
📋 Command-Line Options:
| Option              | Description                 | Example                          |
| ------------------- | --------------------------- | -------------------------------- |
| `-i`, `--interface` | Network interface to modify | `-i eth0` or `--interface wlan0` |
| `-m`, `--mac`       | New MAC address to assign   | `-m 00:11:22:33:44:55`           |

You can view the help message using:

    python mac_changer.py --help
