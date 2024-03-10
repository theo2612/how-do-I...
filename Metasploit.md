# Metasploit Cheat Sheet

## Beginner Concepts

### Basic Usage
```bash
# Basic Usage
msfconsole

# Search for Modules
search <keyword>
# Search for Exploits
search type:exploit platform:windows
# Search for Payloads
search type:payload arch:x86
# Search for Auxillary Modules
search type:auxiliary name:scanner
# Search for Post-Exploitation Modules
search type:post platform:linux

# Use a Module
use <module_name>

# Set Module Options
set <option_name> <value>

# Show Module Options
show options

# Exploit Target
exploit

# Payloads
show payloads

```

### Intermediate
```bash
# Background Session
background

# Multi-Handler
use exploit/multi/handler

# Listener Options
set PAYLOAD <payload_name>
set LHOST <listener_host>
set LPORT <listener_port>

# Custom Payloads
msfvenom -p <payload_name> ...

# Resource Script
resource <script_file>

# Database Integration
db_status
db_connect <database_url>

# Post Exploitation
use post/<module_name>

```
