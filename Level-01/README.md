# Bandit Level 00 → 01

## Objective

Connect to the OverTheWire Bandit server as `bandit0` and find the password for the next level.

## Step 1 — Connect to the Server

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

- `ssh` → Secure Shell; connects to a remote server
- `bandit0` → username
- `bandit.labs.overthewire.org` → server hostname
- `-p 2220` → use port 2220

Enter the Level 00 password when prompted.

## Step 2 — List the Files

```bash
ls
```

Output:

```text
readme
```

`ls` lists files and directories in the current directory.

## Step 3 — Read the `readme` File

```bash
cat readme
```

- `cat` → displays file contents
- `readme` → the file to read

The output contains the password required for Level 01.

## Step 4 — Exit Level 00

```bash
exit
```

This disconnects from the Bandit server and returns to your Mac terminal.

## Step 5 — Connect to Level 01

From your Mac terminal:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

Enter the password obtained from `cat readme`.

**Important:** Do not run the Level 01 SSH command from inside `bandit0`. Exit first, then connect from your Mac.

## Complete Solution

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
ls
cat readme
exit
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

## Key Concepts

- SSH
- Remote Linux server
- SSH usernames
- SSH ports
- `ls`
- `cat`
- `exit`

## What I Learned

- How to connect to a remote Linux server using SSH.
- How to specify a custom SSH port.
- How to list files using `ls`.
- How to read files using `cat`.
- How to disconnect from an SSH session using `exit`.
- The next-level SSH connection should be initiated from the local machine.

## Security Note

Do not commit Bandit passwords to GitHub.

## Next Level

[Level 01 → 02](../Level-01/)
