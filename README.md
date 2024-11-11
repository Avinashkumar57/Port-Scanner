# Port-Scanner
A simple command-line tool for scanning TCP and UDP ports on a target machine. This script allows users to scan a range of ports and identify open ones.
# Features

    TCP and UDP port scanning.
    Customizable port range (--start-port and --end-port).
    Provides basic error handling (e.g., for invalid IP addresses or interrupted scans).
    Easy-to-use command-line interface.

## Installation

    Clone or download this repository to your local machine.

    git clone https://github.com/Avinashkumar57/port-scanner.git
    cd port-scanner

    Ensure you have Python 3 installed. If not, download and install it from the official Python website: python.org.

    There are no additional dependencies required for this script, as it only uses Python's built-in libraries (socket, argparse, and datetime).

## Usage

You can run the script from the command line by passing the target IP address (or hostname), the start and end port range, and optionally, the scan type (TCP or UDP).
# Syntax

python port_scanner.py <target> [--start-port <start>] [--end-port <end>] [--type <tcp/udp>]

## Arguments

    <target>: The target IP address or hostname to scan.
    --start-port <start>: The starting port for the scan. Default is 1.
    --end-port <end>: The ending port for the scan. Default is 65535.
    --type <tcp/udp>: Type of scan to perform. Can be either tcp (default) or udp.

## Example Usage
    Scan TCP ports from 1 to 100 on a specific IP address:
    
    python port_scanner.py 0.0.0.0 --start-port 1 --end-port 100 --type tcp


If the scan is interrupted by the user or encounters an error, appropriate error messages will be shown.
## Error Handling

    KeyboardInterrupt: If the scan is interrupted by the user (e.g., pressing Ctrl + C).
    socket.gaierror: If the target hostname cannot be resolved.
    socket.error: If there is an issue connecting to the target machine.


# Contributing

Feel free to fork this repository and submit pull requests. If you find any bugs or have suggestions, open an issue, and we’ll try to address it promptly.
# Acknowledgments

    This project was inspired by the need for a simple and customizable port scanning tool.
    Special thanks to the Python community for its rich set of libraries and resources.
