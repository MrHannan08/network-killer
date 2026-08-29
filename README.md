Network Killer

Network Killer is an educational Python-based network stress-testing and traffic-generation lab tool built around a simple interactive terminal interface.

The project provides multiple network testing modes, configurable traffic speed, runtime statistics, and a straightforward CLI experience. It is intended for cybersecurity learning, networking experiments, and authorized laboratory environments.

«⚠️ Educational & Authorized Use Only

Use this project only on systems, networks, and services that you own or have explicit permission to test. Unauthorized traffic generation or service disruption may be illegal and can cause real-world impact.»

---

Features

- Interactive terminal-based interface
- Hacker-style CLI design
- UDP traffic testing
- TCP connection testing
- ICMP/ping testing
- HTTP request testing
- Combined testing mode
- Configurable traffic speed
- Runtime packet/request counters
- Thread-based execution
- Operating-system detection
- Basic administrator/root detection
- Start and stop controls
- Runtime status information
- Works with Python 3

---

Requirements

You need:

- Python 3.8 or newer
- Windows, Linux, or a compatible Unix-like environment
- Terminal/Command Prompt
- Network access for network-based testing

No external Python packages are required by the current version.

---

Installation

Linux

Clone the repository:

git clone https://github.com/MrHannan08/network-killer.git

Enter the project directory:

cd network-killer

Run the tool:

python3 network-killer.py

If your script has a different filename, replace "network-killer.py" with the actual filename.

---

Termux Installation

Network Killer can also be used from Termux for authorized laboratory testing.

1. Install Termux

Use a trusted and current Termux distribution.

After opening Termux, update the packages:

pkg update && pkg upgrade

2. Install Python and Git

pkg install python git

Check the installations:

python --version

git --version

3. Clone the Repository

git clone https://github.com/MrHannan08/network-killer.git

Move into the project:

cd network-killer

4. Run the Script

python network-killer.py

If the script uses another filename, run that file instead.

---

Termux Notes

Some network operations behave differently on Android/Termux compared with a traditional Linux system.

In particular:

- ICMP functionality can be restricted by Android.
- Raw networking operations may require privileges that normal Termux does not have.
- Some operations may behave differently depending on the Android version.
- Running as root is not required for ordinary Python execution.
- Do not use Termux to generate unauthorized traffic against public services or networks.

For learning, a controlled local lab or authorized test environment is recommended.

---

Usage

After launching the program, an interactive menu is displayed.

Example:

[1] UDP Flood
[2] TCP Flood
[3] ICMP Flood
[4] HTTP Flood
[5] ALL Combined
[6] Speed Limiter
[7] Stop Attack
[s] Status
[q] Exit

Choose an option by entering its corresponding number or command.

Status

Use:

s

to view runtime information such as:

- Current status
- Packet/request counter
- Number of threads
- Uptime
- Operating system

Exit

Use:

q

to exit the application.

---

How It Works

The application is written entirely in Python and uses Python's built-in modules for its core functionality.

Networking

The "socket" module is used for network communication and connection testing.

Threading

The "threading" module allows different test routines to execute independently.

ICMP

The application uses the system "ping" command for ICMP-related testing.

HTTP

Python's standard-library HTTP functionality is used for HTTP request testing.

Platform Detection

The "platform" module is used to identify the operating system and system version.

Terminal Interface

ANSI escape sequences are used to provide colored terminal output and improve the CLI experience.

---

Project Structure

network-killer/
│
├── network-killer.py
├── README.md
├── .gitignore
└── LICENSE

---

Educational Use Cases

This project can be useful for learning about:

- Python networking
- TCP and UDP communication
- Network traffic generation
- Socket programming
- HTTP requests
- ICMP concepts
- Python threading
- CLI application development
- Basic network monitoring
- Cybersecurity laboratory experimentation

---

Safe Testing Environment

The safest way to experiment with network traffic generation is to create an isolated laboratory.

For example:

┌─────────────────────┐
│    Test Machine     │
│  Network Killer     │
└──────────┬──────────┘
           │
           │ Isolated Network
           │
┌──────────▼──────────┐
│   Authorized Test   │
│       System        │
└─────────────────────┘

Use your own machines, localhost-based environments, virtual machines, or another environment where you have explicit authorization.

---

Security & Responsible Use

Network traffic-generation tools can have unintended consequences when used incorrectly.

Before testing:

1. Make sure you have permission.
2. Know exactly which system is being tested.
3. Use an isolated environment whenever possible.
4. Start with conservative testing parameters.
5. Monitor CPU, memory, bandwidth, and network availability.
6. Stop the test if unexpected behavior occurs.

The author is not responsible for damage, service disruption, data loss, or other consequences resulting from unauthorized or improper use of this project.

---

Limitations

The current version is intentionally a simple CLI-based project.

Possible limitations include:

- Platform-dependent networking behavior
- ICMP restrictions on some systems
- Android/Termux networking restrictions
- Basic error handling
- Limited configuration options
- Runtime-only statistics
- No persistent logging system

---

Future Improvements

Possible improvements for future releases include:

- Dedicated safe laboratory mode
- Localhost-only testing mode
- Configuration files
- Better logging
- Improved statistics
- Session reports
- More robust thread management
- Better cross-platform support
- Automated tests
- Improved error handling
- Configurable testing profiles
- Cleaner CLI architecture

---

Contributing

Contributions, suggestions, and improvements are welcome.

If you want to contribute:

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Test your changes in an authorized environment.
5. Submit a pull request.

For larger changes, opening an issue first is recommended.

---

License

This project is released under the MIT License.

See the "LICENSE" file for the complete license text.

---

Author

MrHannan08

GitHub:

"https://github.com/MrHannan08"

Network Killer is developed as an educational cybersecurity and networking project.

---

Disclaimer

Network Killer is provided for educational and authorized security-testing purposes only.

Do not use this software against systems or networks without explicit permission.

By using this project, you are responsible for ensuring that your activities comply with applicable laws, regulations, and the policies of the networks and services you interact with.

---

⭐ If this project helped you learn about Python networking or cybersecurity, consider giving the repository a star.
