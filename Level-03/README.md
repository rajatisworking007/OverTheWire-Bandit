# ⚔️ Bandit Level 02 → 03

## 🎯 Objective

Find the password stored in a file whose name contains spaces and special characters.

## 1. Connect to Level 02

```bash
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

- `ssh` → secure remote connection
- `bandit2` → username
- `bandit.labs.overthewire.org` → Bandit server
- `-p 2220` → SSH port

## 2. List the files

```bash
ls
```

You should see:

```text
--spaces in this filename--
```

## 3. Why this fails

```bash
cat spaces in this filename
```

The shell separates the filename at every space.

It is interpreted approximately as:

```text
spaces
in
this
filename
```

So `cat` searches for multiple files.

## 4. Correct command

The exact filename starts with `--`, so use:

```bash
cat "./--spaces in this filename--"
```

### Why `./`?

The filename starts with `--`, which can be interpreted as an option by a command.

`./` explicitly means:

> Use the file from the current directory.

## 5. Get the password

```bash
cat "./--spaces in this filename--"
```

The output is the password for Level 03.

## 6. Exit

```bash
exit
```

## 7. Connect to Level 03

From your local terminal:

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```

## 🧠 Key Concepts

- Filenames can contain spaces.
- Quotes keep spaces together as one argument.
- `./` is useful when a filename starts with `-`.
- `cat` prints file contents.

> ⚠️ Never put your actual Bandit password in a public GitHub repository.
