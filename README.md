# codtech-task2
## Basic Vulnerability Scanning Tool <br>
### Overview:
This project is a simple Python-based vulnerability scanning tool designed to identify common security vulnerabilities in a target network or web application. The tool performs two main tasks:

1.Port Scanning: Uses Nmap to scan the target machine for open ports, specifically in the range of 1-1024. This helps identify services running on the target and their potential vulnerabilities.

2.Software Version Check: Sends HTTP requests to the target web server to retrieve the Server header. The tool then checks if the web server software might be outdated by comparing it against known versions.

Features:
-Port Scanning: Identifies open ports and their states (open, filtered, closed) on the target machine.
-Software Fingerprinting: Checks the web server's software and version using the HTTP Server header.
-Error Handling: Provides detailed error messages if there are issues connecting to the target or scanning ports.

Example Output:
![CODTECH Task 2](https://github.com/user-attachments/assets/df49e46d-ed0f-475c-ae8a-0c1e24f758ba)

