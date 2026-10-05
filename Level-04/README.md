# ⚔️ Bandit Level 03 → 04

## 🎯 Objective

Find the password inside the `inhere` directory.

## 1. Connect to Level 03

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```

## 2. List the files

```bash
ls
```

You should see:

```text
inhere
```

`inhere` is a directory.

## 3. Enter the directory

```bash
cd inhere
```

- `cd` → change directory
- `inhere` → directory you want to enter

## 4. Show hidden files

```bash
ls -la
```

### What does `-la` mean?

- `-l` → long listing
- `-a` → show all files, including hidden files

You should find a hidden file similar to:

```text
.hidden
```

Files beginning with `.` are hidden by default.

## 5. Read the hidden file

```bash
cat .hidden
```

The output is the password for Level 04.

## 6. Exit

```bash
exit
```

## 7. Connect to Level 04

From your local terminal:

```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```

## 🧠 Key Concepts

- `cd` changes directories.
- `ls -la` reveals hidden files.
- A filename beginning with `.` is hidden.
- `cat` displays file contents.

> ⚠️ Never publish your actual Bandit password in GitHub.
