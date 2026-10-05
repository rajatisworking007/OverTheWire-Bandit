<div align="center">

# ⚔️ OVER THE WIRE — BANDIT

### `LINUX // CTF // CYBERSECURITY // TERMINAL`

**Enter the terminal. Break the level. Steal the flag. Level up.**

[![Bandit](https://img.shields.io/badge/OverTheWire-Bandit-black?style=for-the-badge)](https://overthewire.org/wargames/bandit/)
[![Linux](https://img.shields.io/badge/Linux-Command_Line-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://www.linux.org/)
[![Bash](https://img.shields.io/badge/Bash-Scripting-121011?style=for-the-badge&logo=gnubash&logoColor=white)](https://www.gnu.org/software/bash/)

</div>

---

## 🎮 MISSION

This repository documents my journey through the **OverTheWire Bandit** wargame.

Bandit is a practical Linux and cybersecurity challenge where every level introduces a new command, concept, vulnerability, or problem-solving technique.

```text
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   PLAYER: RAJAT                                             │
│   MODE:   CYBER TRAINING                                    │
│   GAME:   BANDIT                                            │
│                                                             │
│   OBJECTIVE: COMPLETE EVERY LEVEL                           │
│                                                             │
│   [ TERMINAL ] ──→ [ DISCOVER ] ──→ [ EXPLOIT ] ──→ [ NEXT ]│
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

# 🗺️ LEVEL MAP

> **37 LEVELS • ONE TERMINAL • NO SHORTCUTS**

| Level | Status | Level | Status | Level | Status |
|:---:|:---:|:---:|:---:|:---:|:---:|
| `00` | ⬜ | `13` | ⬜ | `26` | ⬜ |
| `01` | ⬜ | `14` | ⬜ | `27` | ⬜ |
| `02` | ⬜ | `15` | ⬜ | `28` | ⬜ |
| `03` | ⬜ | `16` | ⬜ | `29` | ⬜ |
| `04` | ⬜ | `17` | ⬜ | `30` | ⬜ |
| `05` | ⬜ | `18` | ⬜ | `31` | ⬜ |
| `06` | ⬜ | `19` | ⬜ | `32` | ⬜ |
| `07` | ⬜ | `20` | ⬜ | `33` | ⬜ |
| `08` | ⬜ | `21` | ⬜ | `34` | ⬜ |
| `09` | ⬜ | `22` | ⬜ | `35` | ⬜ |
| `10` | ⬜ | `23` | ⬜ | `36` | ⬜ |
| `11` | ⬜ | `24` | ⬜ | | |
| `12` | ⬜ | `25` | ⬜ | | |

### XP PROGRESS

```text
[░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░]

0 / 37 LEVELS COMPLETED
```

Update the progress bar as you complete levels.

---

# 🧩 WHAT'S INSIDE?

Every level is documented like a game mission:

```text
┌──────────────────────────────────────┐
│  🎯 OBJECTIVE                        │
│  What does the level want?           │
├──────────────────────────────────────┤
│  🔎 RECON                            │
│  What did I investigate?             │
├──────────────────────────────────────┤
│  💻 COMMANDS                         │
│  What commands solved it?            │
├──────────────────────────────────────┤
│  🧠 WHY IT WORKS                     │
│  The actual technical explanation.   │
├──────────────────────────────────────┤
│  🏆 KEY TAKEAWAY                     │
│  What did I learn?                   │
└──────────────────────────────────────┘
```

---

# 🧠 SKILL TREE

```text
                         ┌───────────────┐
                         │   BANDIT      │
                         └───────┬───────┘
                                 │
              ┌──────────────────┼──────────────────┐
              ▼                  ▼                  ▼
        ┌───────────┐      ┌───────────┐      ┌───────────┐
        │   LINUX   │      │ NETWORKS  │      │ SECURITY  │
        └─────┬─────┘      └─────┬─────┘      └─────┬─────┘
              │                  │                  │
       ┌──────┼──────┐      ┌────┼────┐       ┌─────┼─────┐
       ▼      ▼      ▼      ▼         ▼       ▼     ▼     ▼
      Bash   Files  Perms  SSH       Ports  Auth  Crypto  PrivEsc
       │      │      │      │         │       │     │       │
       └──────┴──────┴──────┴─────────┴───────┴─────┴───────┘
                              │
                              ▼
                       🛡️ CYBERSECURITY
```

---

# 🛠️ COMMAND ARSENAL

Commands encountered throughout the journey may include:

```bash
# Navigation
pwd
ls
cd

# Files
cat
less
head
tail
file
find
strings

# Text processing
grep
sort
uniq
cut
tr
diff

# Permissions
chmod
chown
ls -la

# Networking
ssh
nc
nmap

# Encoding / Crypto
base64
openssl
xxd

# Processes / System
ps
top
env
whoami

# Automation
cron
crontab

# Shell
bash
sh
```

> Commands are not just syntax. The goal is to understand **why** they work.

---

# 📁 REPOSITORY STRUCTURE

```text
OverTheWire-Bandit/
│
├── README.md
│
├── Level-00/
│   └── README.md
│
├── Level-01/
│   └── README.md
│
├── Level-02/
│   └── README.md
│
├── ...
│
└── Level-36/
    └── README.md
```

Each level gets its own write-up.

---

# 🧪 LEVEL WRITE-UP FORMAT

Each level follows this structure:

```markdown
# Bandit Level XX → XX

## 🎯 Objective

## 🔎 Recon / Approach

## 💻 Commands Used

## 🧠 Command Breakdown

## ⚙️ Why It Works

## 🏆 Key Concepts

## 📌 What I Learned

## ⚠️ Mistakes / Troubleshooting

## ➡️ Next Level
```

The objective is to document the **reasoning**, not just paste a command.

---

# 🔐 PASSWORD POLICY

Passwords are **not stored in this repository**.

The repository documents:

- Commands
- Techniques
- Reasoning
- Linux concepts
- Security concepts
- Troubleshooting

Secrets stay out of Git.

---

# 🕹️ PLAYER RULES

```text
RULE 01 ── Try the level yourself first.

RULE 02 ── Understand every command you execute.

RULE 03 ── Don't blindly copy solutions.

RULE 04 ── Document mistakes.

RULE 05 ── Never commit passwords or credentials.

RULE 06 ── Move to the next level only after understanding the current one.
```

---

# 📈 JOURNEY

```text
LEVEL 00
   ↓
Linux Fundamentals
   ↓
File & Permission Handling
   ↓
Text Processing
   ↓
Networking
   ↓
SSH / Services
   ↓
Encoding & Cryptography
   ↓
Shell Scripting
   ↓
Privilege Concepts
   ↓
LEVEL 36
   ↓
╔══════════════════════════════╗
║      BANDIT COMPLETED        ║
╚══════════════════════════════╝
```

---

# 🎯 WHY I'M DOING THIS

The purpose of this repository is not just to finish a CTF.

It is to build practical foundations for:

```text
Linux
  ↓
Networking
  ↓
Cybersecurity
  ↓
Web Security
  ↓
Cloud Security
  ↓
Security Engineering
```

---

# 🔗 RESOURCES

- **OverTheWire:** https://overthewire.org/
- **Bandit:** https://overthewire.org/wargames/bandit/

---

<div align="center">

### `> ACCESS GRANTED_`

**37 LEVELS. ONE TERMINAL. KEEP LEARNING.**

```text
██████╗  █████╗ ███╗   ██╗██████╗ ██╗████████╗
██╔══██╗██╔══██╗████╗  ██║██╔══██╗██║╚══██╔══╝
██████╔╝███████║██╔██╗ ██║██║  ██║██║   ██║
██╔══██╗██╔══██║██║╚██╗██║██║  ██║██║   ██║
██████╔╝██║  ██║██║ ╚████║██████╔╝██║   ██║
╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═══╝╚═════╝ ╚═╝   ╚═╝
```

</div>
