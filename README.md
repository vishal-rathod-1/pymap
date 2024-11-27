##Pymap - Nmap CLI Tool

Pymap is a simple Python CLI tool to run full Nmap scans on a target and save results in a text file. This tool supports features like port scanning, OS detection, vulnerability scanning, and more.

Installation

To use this tool, you can either clone the repository or download the Python file.

##Install Prerequisites

Python 3.x: Make sure Python 3.x is installed. You can verify this with:

python3 --version

Nmap: Install Nmap on your machine.

#On Linux (Ubuntu/Debian):

sudo apt-get install nmap

#On macOS (using Homebrew):
brew install nmap
Required Python Modules: The subprocess and argparse modules are built-in, but if you run into any issues, you can install them using:


pip3 install subprocess argparse

Make the Script Executable
After downloading the pymap.py file, you need to make it executable by running:

chmod +x pymap.py
This will allow you to execute the script directly from the command line.

Usage
Once installed, you can use Pymap to run Nmap scans on your desired target.

Run the following command to start a scan:

sudo ./pymap.py -u <target_url> -p <port_range>
Where:

-u <target_url>: The URL or IP address of the target you wish to scan.
-p <port_range>: The range of ports to scan (e.g., -p 22-80 to scan ports 22 through 80).
Example

sudo ./pymap.py -u example.com -p 22-80
