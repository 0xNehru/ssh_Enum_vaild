# ssh_Enum_vaild
A Bash script to enumerate valid SSH usernames using the CVE-2018-15473 vulnerability. It checks for valid usernames on an OpenSSH server by analyzing authentication responses.

# Features

✅ Detects valid SSH usernames based on OpenSSH response behavior
✅ Uses a public key authentication bypass technique
✅ Optimized for speed using parallel processing
✅ Saves valid usernames automatically to valid_usernames.txt
✅ Lightweight, requires only Bash and OpenSSH client

1. Only displays valid usernames (removes invalid ones from output).
2. Saves valid usernames to valid_usernames.txt.
3. Runs faster by executing checks in parallel.
# Usage
chmod +x exploit.sh

./exploit <target> <port> <username_file> 

Example:

./exploit 192.168.1.1 22 usernames.txt

# Requirements

    1.Linux/macOS with Bash
    2.OpenSSH client (ssh, ssh-keygen, nc)
    3.Target system running OpenSSH

⚠️ Disclaimer

This script is for educational and authorized security testing only. Do not use it on systems without permission.

🔗 CVE-2018-15473 Details
