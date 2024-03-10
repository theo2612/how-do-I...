# Bash Cheat Sheet

## Beginner Concepts

### Basic Commands
```bash
# Basic Commands
pwd         # Print current directory
ls          # List directory contents
cd          # Change directory
mkdir       # Make directory
touch       # Create empty file

# File Operations
cat         # Display file content
cp          # Copy files and directories
mv          # Move or rename files and directories
rm          # Remove files and directories

# Text Manipulation
echo        # Print message
grep        # Search text
sed         # Stream editor
awk         # Text processing

# Text Manipulation
echo        # Print message
grep        # Search text
sed         # Stream editor
awk         # Text processing

# Permissions
chmod       # Change file permissions
chown       # Change file ownership
chgrp       # Change group ownership

# Environment Variables
export      # Set environment variables
env         # Display environment variables
```

## Intermediate Concepts
```bash
# Shell Scripting
#!/bin/bash  # Shebang line
$1, $2, ...  # Positional parameters
if ...; then
    # Code block
fi

# Conditional Statements
if ...; then
    # Code block
elif ...; then
    # Code block
else
    # Code block
fi

# Loops
for ...; do
    # Code block
done

while ...; do
    # Code block
done

# Functions
function_name() {
    # Code block
}
function_name   # Call function

# Command Substitution
variable=$(command)

# Job Control
&           # Run command in background
jobs        # List background jobs
fg          # Bring job to foreground
bg          # Resume job in background

# Redirection and Pipes
>           # Redirect output to file
>>          # Append output to file
<           # Redirect input from file
|           # Pipe output to another command

# Conditionals and Loops with Advanced Commands
find ... -exec ... \;    # Execute command for each file found
xargs ...                # Build and execute command lines from standard input


```

