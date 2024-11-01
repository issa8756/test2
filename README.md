# Toolbox for Penetration Testing

This project contains a collection of Python scripts that can be used for penetration testing and IT security. It includes five main tools, each utilizing an external library to provide advanced functionality.

## Project Contents

- `main_script.py`: Main script to invoke the different tools.
- `encrypt_tool.py`: Tool for encryption and decryption.
- `nmap_scanning_tool.py`: Tool for network scanning using Nmap.
- `brute_force_tool.py`: Tool for password cracking using brute force.
- `text_replacement_tool.py`: Tool for replacing specific patterns in text (e.g., phone numbers, emails, dates).


## How to Use

To run the tools, use the `main_script.py` with the desired tool option. Here’s how to use each tool:

### 1. Encrypt Tool

This tool allows you to generate encryption keys and encrypt/decrypt files.

**Usage Example:**

```bash
python main_script.py encrypt_tool generate_key
python main_script.py encrypt_tool encrypt myfile.txt
python main_script.py encrypt_tool decrypt myfile.txt.encrypted
```

### 2. Nmap Scanner Tool

This tool is used to scan networks and identify connected devices using Nmap.

**Usage Example:**

```bash
python main_script.py nmap_scanner_tool -ips 192.168.1.0/24 -t syn -o scan_results.txt -T 4 -p 22,80
```

### 3. Brute Force Tool

This tool is used for password cracking through brute force attacks.

**Usage Example:**

```bash
python main_script.py brute_force_tool 192.168.1.100 normal passwords.txt -u admin
```

### 4. Text Replacement Tool

This tool replaces specific patterns in text, such as phone numbers, email addresses, and dates.

**Usage Example:**

```bash
python main_script.py text_replacement_tool input.txt output.txt -p -e -d
```

## Requirements

- Python 3.x
- Libraries used:
  - `cryptography`
  - `nmap`
  - `argparse` (for command-line argument parsing)
  - `re` (for regular expression operations)

## Installation

Make sure to install the required libraries using:

```bash
pip install cryptography python-nmap
```

## Notes

- Ensure that the necessary input files are present before running the tools.
- When using the Nmap scanner tool, you may need to run the script with elevated privileges (e.g., using `sudo` on Unix-like systems) to perform certain types of scans.
- All logs will be saved in the `main_script.log` file.

## Contribution

If you have any suggestions or improvements, feel free to contribute!
