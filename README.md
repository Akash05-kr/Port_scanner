# Port Scanner

This Python script is a simple port scanner that scans a specified number of ports on a target IP address or domain name. It retrieves banner information from open ports and checks for known vulnerabilities based on predefined banners.

## Features

- Scans a range of ports on a specified target.
- Retrieves service/version information (banner) from open ports.
- Checks retrieved banners against a list of known vulnerable banners.
- Prints out any identified vulnerabilities.

## Prerequisites

- Python 3.x
- IPy library (`pip install IPy`)

## Usage

1. **Clone the repository:**
git clone <repository-url>

2. **Navigate to the directory:**
cd port-scanner

3. **Install dependencies:**
pip install IPy

4. **Run the script:**
python port_scanner.py

5. **Follow the prompts:**
- Enter the target IP address, localhost, or domain name when prompted.
- Enter the number of ports to scan.

6. **View results:**
- The script will output any identified vulnerabilities based on the banners retrieved.

## Example

Enter Target IP address, localhost or www.domainname.com : www.example.com
Enter Number of ports to be scanned: 100

## Notes

- Adjust the timeout (`s.settimeout(5)`) in `port_scanner` function as needed for your network environment.
- Ensure `vulnarable_banners.txt` contains the correct list of vulnerable banners for accurate vulnerability detection.


