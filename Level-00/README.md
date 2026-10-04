# Bandit Level 00 → Level 01

## 🎯 Objective

The objective of Level 0 is to connect to the **OverTheWire Bandit server** using SSH.

This level introduces the basics of:

- SSH
- Remote Linux servers
- Usernames
- Hostnames
- Network ports

---

## 🖥️ Step 1 — Connect to the Server

Run:

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

### Command Breakdown

```text
ssh
```

`ssh` stands for **Secure Shell**. It is used to securely connect to a remote computer.

```text
bandit0
```

This is the username provided for Level 0.

```text
@
```

Separates the username from the server address.

```text
bandit.labs.overthewire.org
```

This is the hostname of the OverTheWire Bandit server.

```text
-p
```

Specifies the port that SSH should use.

```text
2220
```

Port `2220` is the SSH port used by the Bandit game.

---

## 🔐 Step 2 — Authentication

After running the command, SSH may ask whether you trust the server.

```text
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```

Enter:

```text
yes
```

SSH will then ask for the Level 0 password:

```text
bandit0@bandit.labs.overthewire.org's password:
```

Enter the password provided by OverTheWire.

> Passwords are intentionally not stored in this repository.

---

## ✅ Step 3 — Verify the Connection

After successful authentication, the terminal will show a prompt similar to:

```text
bandit0@bandit:~$
```

This means we are successfully logged into the Bandit server as `bandit0`.

---

## 🧠 Understanding the Prompt

```text
bandit0@bandit:~$
```

| Part | Meaning |
|---|---|
| `bandit0` | Current username |
| `@` | Separates user and host |
| `bandit` | Remote machine |
| `~` | User's home directory |
| `$` | Normal user shell |

---

## 💻 Command Used

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

---

## 📚 Key Concepts Learned

### SSH

SSH allows us to securely access and control a remote computer through a command-line interface.

### Port

A port identifies a network service running on a machine.

Bandit uses:

```text
Port: 2220
```

instead of the default SSH port:

```text
Port: 22
```

### Remote Login

Instead of working on our own Mac, we are now working inside a remote Linux server.

---

## 📝 What I Learned

- How to connect to a remote Linux machine.
- How SSH authentication works.
- How usernames and hostnames are used.
- How to specify a custom SSH port.
- How to identify the current user and remote machine from the shell prompt.

---

## ➡️ Next Level

After successfully connecting as `bandit0`, Level 1 requires finding the password stored in the `readme` file.

[Go to Level 01 →](../Level-01/)
