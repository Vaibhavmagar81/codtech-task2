**Name: Vaibhav Magar<br>
Company:CODTECH IT SOLUTIONS <br>
ID:CT4CSEH6043 <br>
Domain:Cyber Security <br>
Duration:1 Aug to 1 Sep <br>
Mentor:Muzammil Ahmed <br>**

# codtech-task2
## Basic Vulnerability Scanning Tool <br>
### Overview:
This project is a simple Python-based vulnerability scanning tool designed to identify common security vulnerabilities in a target network or web application. The tool performs two main tasks:

### Import Required Modules:

**nmap**: Used for scanning open ports on the target machine.<br>
**requests**: Used for sending HTTP requests to check the server's software version.

## Functions Defined:
### scan_open_ports(target):
- Scans the specified target for open ports in the range 1-1024 using Nmap.
- It prints out the host's state, the protocol used, and the status (open/filtered/closed) of each port.
- Error handling is included to catch any exceptions during the scanning process.

### check_software_version(url, known_versions):
- Sends an HTTP request to the target URL.
- Checks the Server header in the HTTP response to identify the web server software and its version.
- Compares the version in the Server header with a known list of expected versions to see if the software might be outdated.
- Handles connection errors gracefully, printing an appropriate error message if the connection fails.

### Main Execution Block:
- Prompts the user to enter a target IP address or domain.
- Calls scan_open_ports() to identify and print open ports on the target.
- Defines a dictionary known_versions containing some common web server software and their expected versions.
- Constructs a URL using the target and checks for software versions using check_software_version().

### Error Handling:
Both functions include error handling to manage potential exceptions, such as failed connections or scanning issues, providing helpful output to the user.

### Usage:
- The script is intended to be run from the command line, where the user inputs the target IP or domain.
- It provides basic security information by identifying open ports and checking for potentially outdated web server software based on the Server header.
- This code is a simple tool for preliminary vulnerability scanning, particularly useful for identifying open ports and basic web server fingerprinting.

### Output:
![CODTECH Task 2](https://github.com/user-attachments/assets/df49e46d-ed0f-475c-ae8a-0c1e24f758ba)

