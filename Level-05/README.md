# ⚔️ Bandit Level 04 → 05

## 🎯 Objective

Inside the `inhere` directory, find the only file containing human-readable text.

## 1. Connect to Level 04

```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```

## 2. List the directory

```bash
ls
```

You should see:

```text
inhere
```

## 3. Enter the directory

```bash
cd inhere
```

## 4. Show all files

```bash
ls -la
```

You should see multiple files with names similar to:

```text
-file00
-file01
-file02
...
-file09
```

## 5. Identify the file type

The normal approach is:

```bash
file ./*
```

- `file` → identifies the type of data
- `./*` → checks files in the current directory

Look for the file reported as:

```text
ASCII text
```

That is the human-readable file.

## 6. If `file` does not work

Try:

```bash
/usr/bin/file ./*
```

Alternative:

```bash
find . -type f -exec grep -Il . {} \;
```

This can identify files containing readable text.

## 7. Read the identified file

Suppose the command identifies:

```text
./-file07
```

Then run:

```bash
cat ./-file07
```

**Important:** Do not blindly use `-file07`. Use the filename actually returned by your command.

## 8. Get the password

The output of the correct file is the password for Level 05.

## 9. Exit

```bash
exit
```

## 10. Connect to Level 05

From your local terminal:

```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
```

## 🧠 Key Concepts

- `file` identifies file types.
- `./*` targets files in the current directory.
- `find` searches for files.
- `grep -I` can help identify text files.
- `cat` reads the selected file.

> ⚠️ Never publish your actual Bandit password in GitHub.
