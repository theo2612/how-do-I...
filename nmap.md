# Nmap Cheat Sheet

## Beginner Concepts

### Basic Scanning
```bash
# Basic Scanning
nmap <target>      # Scan a single target
nmap <target1> <target2>  # Scan multiple targets

# Scan Types
nmap -sP <target>       # Ping scan (discover hosts)
nmap -sS <target>       # TCP SYN scan
nmap -sT <target>       # TCP connect scan
nmap -sU <target>       # UDP scan
nmap -sV <target>       # Version detection

# Scan Options
nmap -p <port> <target>     # Scan specific port(s)
nmap -F <target>            # Fast scan (100 most common ports)
nmap -T<0-5> <target>       # Timing template (0-5, higher is faster)
nmap -A <target>            # Aggressive scan (OS detection, version detection, script scanning)

# Output Options
nmap -oN output.txt <target>   # Output to normal format
nmap -oX output.xml <target>   # Output to XML format
nmap -oG output.grep <target>  # Output to grepable format
```

## Intermediate Concepts
```bash
# Scripting Engine
nmap --script <script> <target>     # Run specific NSE script(s)
nmap --script-help <script>         # Get help for NSE script

# OS Detection
nmap -O <target>            # Perform OS detection

# Firewall Evasion
nmap -f <target>            # Fragment packets
nmap --mtu <MTU> <target>  # Specify MTU size

# Timing and Performance
nmap -T<0-5> <target>       # Timing template (0-5, higher is faster)
nmap --max-rtt-timeout <time> <target>   # Maximum round trip time timeout

# Scan Optimization
nmap --min-parallelism <num> <target>    # Minimum parallelism level
nmap --min-hostgroup <num> <target>      # Minimum number of hosts per group

# Output Filtering
nmap --open <target>        # Show only open ports
nmap --closed <target>      # Show only closed ports
nmap --host-timeout <time> <target>   # Host timeout value


```
