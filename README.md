# Prodigy_CS_05

# Scapy Packet Capture Tool

## Overview

The Scapy Packet Capture Tool is a Python script designed to capture and log details of IP packets using the Scapy library. It captures packets on the default network interface and logs the protocol type, source IP address, destination IP address, and additional protocol-specific details.

## Features

- Captures IP packets on the default network interface.
- Logs protocol type, source IP, destination IP, and additional details for TCP, UDP, and ICMP packets.
- Supports logging to a file for better analysis.
- Includes error handling for robust packet processing.

## Requirements

- Python 3.x
- Scapy library

## Installation

1. **Clone the repository**:

   ```sh
   git clone https://github.com/your-username/scapy-packet-capture-tool.git
   cd scapy-packet-capture-tool

2. **Install Scapy**:

    ```sh
    pip install scapy

## Usage

1. Run the script:

```sh 
    python packet_capture.py

2. View the log file:

The captured packet details will be logged to packet_capture.log in the same directory.

Example Output
The log file will contain entries similar to the following:


Copy
2025-02-04 12:34:56 - Protocol: TCP
2025-02-04 12:34:56 - Source IP: 192.168.1.1
2025-02-04 12:34:56 - Destination IP: 192.168.1.2
2025-02-04 12:34:56 - TCP Source Port: 1234, Destination Port: 80
--------------------------------------------------
Customization
Filtering: You can modify the sniff function's filter parameter to capture specific types of traffic. For example, to capture only TCP packets:

python

Copy
sniff(prn=packet_callback, filter="tcp", store=0)
Logging: Change the logging configuration in the script to log to a different file or format as needed.

