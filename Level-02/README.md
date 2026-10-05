# Bandit Level 01 → 02

## 🎯 Objective

Find the password for **Level 02**.

The password is stored in a file named:

```text
-
```

The challenge is to correctly read a file whose name is a special character.

---

## 1. Connect to Level 01

From your Mac Terminal:

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
```

Enter the password obtained from **Level 00 → 01**.

---

## 2. List the Files

Run:

```bash
ls
```

You will see:

```text
-
```

The filename is literally a single hyphen.

---

## 3. Why `cat -` Doesn't Work

You might try:

```bash
cat -
```

But this does not read the file.

In Unix/Linux commands, `-` is commonly interpreted as **standard input (stdin)**.

Therefore, `cat -` waits for input from the terminal.

If this happens, press:

```text
Ctrl + C
```

to stop the command.

---

## 4. Read the File Correctly

Use:

```bash
cat ./-
```

### Command Breakdown

```text
cat
```

Displays the contents of a file.

```text
./
```

Refers to the current directory.

```text
-
```

The actual filename.

Therefore:

```bash
cat ./-
```

means:

> Read the file named `-` from the current directory.

The output is the **password for Level 02**.

---

## 5. Connect to Level 02

First exit the current SSH session:

```bash
exit
```

Then, from your **Mac Terminal**, connect to Level 02:

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

Enter the password obtained from:

```bash
cat ./-
```

---

## 💻 Complete Solution

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220

ls

cat ./-

exit

ssh bandit2@bandit.labs.overthewire.org -p 2220
```

---

## 🧠 Key Concepts

| Command | Purpose |
|---|---|
| `ls` | List files and directories |
| `cat` | Display file contents |
| `./` | Current directory |
| `Ctrl + C` | Interrupt a running command |
| `exit` | Close the SSH session |

---

## 🔥 Main Lesson

A filename can conflict with the special syntax understood by a command.

```bash
cat -
```

treats `-` as standard input.

```bash
cat ./-
```

explicitly tells `cat` to read the file named `-`.

---

## 🏆 What I Learned

- How Linux handles special filenames.
- Why `cat -` behaves differently.
- How `./` can explicitly reference a file.
- How to interrupt a command with `Ctrl + C`.
- How to move from one Bandit level to the next.

---

## ➡️ Next Level

[Level 02 → 03](../Level-02/)
