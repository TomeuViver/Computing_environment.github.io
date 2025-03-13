# Preparation of Computing Environments

## Download the Virtual Machine

To begin, you need to download and install a Linux-based virtual machine that includes all necessary data and bioinformatics tools for the workshop.

[Download Virtual Machine](www.google.com)

Once downloaded, follow the installation instructions to set it up on your computer.

---

## Basic Concepts and Command Lines for Using the Terminal

The Linux terminal is a powerful tool for navigating and managing files. Below are essential commands with explanations:

### 1️⃣ Checking Your Position in the Filesystem

```bash
pwd
```
> Prints the current directory you are in.

### 2️⃣ Listing Files and Directories

```bash
ls
```
> Lists the contents of the current directory.

```bash
ls -lh
```
> Displays the directory contents with additional details like size, permissions, and timestamps.

```bash
ls * > list.txt
```
> Saves the output of `ls` to a file called `list.txt`.

```bash
ls * >> list.txt
```
> Appends the output of `ls` to `list.txt` instead of overwriting it.

---

### 3️⃣ Managing Directories

```bash
mkdir my_directory
```
> Creates a new directory called `my_directory`.

```bash
cd my_directory
```
> Moves into `my_directory`. Press `TAB` to autocomplete folder names.

```bash
cd ..
```
> Moves one directory up.

```bash
rm -r my_directory
```
> Deletes the directory and its contents.

---

### 4️⃣ Creating and Editing Files

```bash
vi my_file.txt
```
> Opens `vi` editor to create/edit `my_file.txt`. Press `i` to insert text.

```bash
# Write inside the file: "Hello, my name is Tomeu"
: Ctrl + x  # Save and exit
```

---

### 5️⃣ Copying, Moving, and Removing Files

```bash
cp my_file.txt my_second_file.txt
```
> Copies `my_file.txt` to `my_second_file.txt`.

```bash
mv my_second_file.txt my_directory/
```
> Moves `my_second_file.txt` to `my_directory`.

```bash
rm my_file.txt
```
> Deletes `my_file.txt`.

---

### 6️⃣ Viewing File Contents

```bash
less my_file.fasta
```
> Opens a file for viewing without modifying it.

```bash
less my_file.fasta | head
```
> Displays the first 10 lines of the file.

```bash
tail my_file.fasta
```
> Displays the last 10 lines of the file.

---

### 7️⃣ Concatenating and Searching Within Files

```bash
cat my_file_1.fasta my_file_2.fasta > my_file_CONCAT.fasta
```
> Merges two files into one.

```bash
grep ">" my_file_1.fasta
```
> Searches for lines containing `>` in `my_file_1.fasta`.

```bash
grep -c ">" my_file_1.fasta
```
> Counts occurrences of `>` in `my_file_1.fasta`.

---

### 8️⃣ Search and Replace Text in Files

```bash
sed 's/from/to/g' in_file.txt > out_file.txt
```
> Replaces all instances of `from` with `to` and saves the result in `out_file.txt`.

```bash
sed -i 's/from/to/g' in_file.txt
```
> Replaces text directly in `in_file.txt` without creating a new file.

---

### 9️⃣ Zipping and Unzipping Files

```bash
gzip file_name.fastq
```
> Compresses `file_name.fastq` into `file_name.fastq.gz`.

```bash
gunzip file_name.fastq.gz
```
> Decompresses `file_name.fastq.gz` back to `file_name.fastq`.

---


