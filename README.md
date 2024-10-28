### NebRec : Advanced Web Scanning Tool

NebRec is a Python script designed to be an **Advanced Web Scanning Tool** for comprehensive security assessments of web applications and networks. It utilizes and integrates various popular open-source security tools and libraries to perform comprehensive reconnaissance and vulnerability assessments on web targets, providing a user-friendly interface for conducting multiple security checks and analyses.

Here is a breakdown of the script's features:

*   **Information Gathering**

    *   WHOIS Lookup: Retrieves ownership and registration details of a domain.
    *   DNS Reconnaissance: Performs DNS resolution to obtain IP addresses associated with a domain.
    *   Subdomain Enumeration: Uses Sublist3r to discover subdomains of the target domain.

*   **Security Assessment**

    *   SSL/TLS Security Check: Analyzes the SSL/TLS configuration of the target domain using OpenSSL.
    *   HTTP Security Headers Check: Examines the HTTP security headers returned by the web server.
    *   CMS Detection and Vulnerability Identification: Attempts to identify the Content Management System (CMS) used by the website and checks for known vulnerabilities in plugins.
    *   Parameter Tampering and Injection Point Identification: Identifies potential injection points for parameter tampering attacks.
    *   Web Technology Fingerprinting: Detects the web technologies and their versions used by the target domain.
    *   Search Public Code Repositories: Searches for code related to the domain in public repositories.

*   **Vulnerability Scanning**

    *   Network Scanning: Performs network scanning using Nmap to discover open ports and services.
    *   Nikto Vulnerability Scan: Runs a vulnerability scan using Nikto to identify common security issues.
    *   WAFW00F Scan: Detects the presence of Web Application Firewalls (WAFs) using WAFW00F.
    *   Advanced Nmap Scan (NSE): Conducts a more in-depth scan using Nmap Scripting Engine (NSE) scripts, including vulnerability detection scripts like "vulners".

*   **Reporting**

    *   The script allows users to generate text file reports for most of the scanning and reconnaissance tasks.

*   **User Interface**

    *   The script provides a simple command-line interface (CLI) for user interaction. Users can select from a menu of options to perform different tasks.

*   **Dependencies**

    *   Python libraries: colorama, subprocess, requests, urllib.parse, whois, dns.resolver
    *   External tools: Sublist3r, gobuster, nmap, OpenSSL, Nikto, WAFW00F

    &#x20;

## Installation

### Requirements

- Python 3.x
- Required Python Libraries: `colorama`, `requests`, `python-whois`, `dnspython`, `sublist3r`, `gobuster`, `nmap`, `nikto`, `wafw00f`

### External Tools

- Sublist3r: [Install Sublist3r](https://github.com/aboul3la/Sublist3r)
- Gobuster: [Download Gobuster](https://github.com/OJ/gobuster)
- Nmap: [Download Nmap](https://nmap.org/)
- Nikto: [Download Nikto](https://cirt.net/Nikto2)
- WAFW00F: `pip install wafw00f`

### Windows Installation

1. Install the required Python libraries:
   ```sh
   pip install -r requirements.txt
2. Download and install the external tools. Make sure they are added to your system's PATH environment variable.
3. Extract `NebRec_Windows.zip` and navigate to the extracted directory.
4. Run the `install.bat` script to set up the environment:
   ```sh
   install.bat
5. To uninstall, run the `uninstall.bat` script:
   ```sh
   uninstall.bat

### Linux Installation

1. Install the required Python libraries:
   ```sh
   pip install -r requirements.txt
2. Download and install the external tools. Make sure they are added to your system's PATH environment variable.
3. Extract `NebRec_Linux.zip` and navigate to the extracted directory.
4. Make the `install.sh` and `uninstall.sh` scripts executable:
   ```sh
   chmod +x install.sh
   chmod +x uninstall.sh
5. Run the `install.sh` script to set up the environment:
  ```sh
  ./install.sh
  ```
  
7. To uninstall, run the `uninstall.sh` script:
   ```sh
   ./uninstall.sh

### Usage
1. Open a terminal or command prompt.
2. Navigate to the directory where you saved the NebRec script.
3. Run the script using the command:
   ```sh
   python nebrec.py
4. Follow the on-screen prompts to select the desired scanning options.

### Example
  ```sh
python nebrec.py
Enter the target domain (e.g., example.com): example.com
Select an option:
1. WHOIS Lookup
2. DNS Reconnaissance
...
Enter your choice: 1
  ```
## Features by List
1. WHOIS Lookup
2. DNS Reconnaissance
3. SSL/TLS Security Check
4. HTTP Security Headers Analysis
5. Subdomain Enumeration
6. Directory Enumeration
7. Network Scanning (Nmap)
8. CMS Detection and Plugin Vulnerability Identification
9. Parameter Tampering and Injection Point Identification
10. Web Technology Fingerprinting and Version Detection
11. Nikto Vulnerability Scan
12. WAFW00F Scan
13. Search Public Code Repositories
14. Advanced Nmap Scan (NSE)

### Important Notes
* Ensure that all required external tools are installed and accessible in your system's PATH.

* This tool is intended for ethical security assessments and research purposes only. Using it against targets without proper authorization is illegal and unethical.

* The accuracy and completeness of the scan results may vary depending on factors like network conditions, target configuration, and tool limitations.

### Disclaimer
* This tool is provided as-is, without any warranty or guarantee of any kind. The developers are not responsible for any misuse or damage caused by this tool. Use it responsibly and ethically.


### Note:
Some features, such as CMS Detection, Parameter Tampering, and Public Code Repository Search, are not fully implemented, and their results may be incomplete or inaccurate.

Feel free to tweak this as needed!
   

