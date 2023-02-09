# Experiment 1 : Introduction to Linux Commands

## Aim

To study about various shells of different operating systems and commands to perform different functions and operations.

## Theory

|Description|Commands|
|---|---|
Listing Files and Directories|`ls`
Long and Time Formatted Listing|`ls -alt`
Change home directory to 'path'|`cd path`
Change to home directory|`cd`
Show current working directory|`pwd`
Create a directory 'new'|`mkdir new`
Create a file 'file1.txt'|`touch file1.txt`
Command is used to update the timestamp of a file|`touch`
Command is used to delete files|`rm`
Command is used to concatenate files and print on the monitor|`cat`
Copy files from one directory to another|`cp`
Move files from one directory to another|`mv`

## Lab Exercises

### 1. Explore the file system of a Windows system and a Linux system, and write prime differences

> Ans.
> **File System in Linux**
> Linux supports more than 12 file systems with NFS technology. Ext file system is the most popular option. It is similar to the Berkeley file system. Linux supports the following file types:
>
> 1. **Directory**: This is simply a list of names.
> 2. **Ordinary File**: This is a file containing data or application program or executable.
> 3. **Symbolic Link**: This file is actually a link to(or path of) another file
> 4. **Special File**: This refers to a device driver
> 5. **Named Pipe**: This is a common channel between two or more processes for data exchange.
>
> **File System in Windows**
> Windows 2000 (W2K) supports a number of file systems including FAT. Developers designed a new file system NTFS that is intended to meet high-end requirements.
> **_Key Feature of NTFS_**
>
> 1. Recoverability
> Security
> Large disks and large files
> Multiple data streams
> General Indexing Facility
>
> **_NTFS Volume and File Structure_**
>
> 1. **Sector**: The smallest physical storage unit on the disk.
> 2. **Cluster**: One or more contiguous sectors.
> 3. **Volume**: A logical partition on a disk, consisting of one or more clusters and used by a file system to allocate space.

### 2. Create a file in your Linux system, in your current user's home directory, named as `file1.txt`. Write your name and registration number in the `file1.txt` using `cat` command. Now rename the file using mv command, the new name must be `yourRegistrationNumber.txt`

Ans.

```bash
ruzdan@Ubuntu:~$ touch file1.txt
ruzdan@Ubuntu:~$ ls
Desktop  Documents  Downloads  file1.txt  Music  Pictures  Public  snap  Templates  Videos
ruzdan@Ubuntu:~$ cat > file1.txt 
Ayan Ruzdan
12116032
ruzdan@Ubuntu:~$ ls
Desktop  Documents  Downloads  file1.txt  Music  Pictures  Public  snap  Templates  Videos
ruzdan@Ubuntu:~$ cat file1.txt 
Ayan Ruzdan
12116032
ruzdan@Ubuntu:~$ mv file1.txt 12116032.txt
ruzdan@Ubuntu:~$ ls
12116032.txt  Desktop  Documents  Downloads  Music  Pictures  Public  snap  Templates  Videos
ruzdan@Ubuntu:~$ cat 12116032.txt 
Ayan Ruzdan
12116032
```

### 3. Create a copy of the file you have created with your registration number. Now delete the original file.

Ans.

```bash
ruzdan@Ubuntu:~$ ls
12116032.txt  Documents  Music     Public  Templates
Desktop       Downloads  Pictures  snap    Videos
ruzdan@Ubuntu:~$ cp 12116032.txt 12116032_copy.txt 
ruzdan@Ubuntu:~$ ls
12116032_copy.txt  Desktop    Downloads  Pictures  snap       Videos
12116032.txt       Documents  Music      Public    Templates
ruzdan@Ubuntu:~$ rm 12116032.txt
ruzdan@Ubuntu:~$ ls
12116032_copy.txt  Documents  Music     Public  Templates
Desktop            Downloads  Pictures  snap    Videos
ruzdan@Ubuntu:~$ cat 12116032_copy.txt 
Ayan Ruzdan
12116032
```

### 4. Create a directory with your name and move all the files (using mv command) created by you in currently logged in user's home directory.

Ans.

```bash
ruzdan@Ubuntu:~$ mkdir Ayan
ruzdan@Ubuntu:~$ ls
12116032_copy.txt  Desktop    Downloads  Pictures  snap       Videos
Ayan               Documents  Music      Public    Templates
ruzdan@Ubuntu:~$ mv 12116032_copy.txt Ayan
ruzdan@Ubuntu:~$ ls
Ayan     Documents  Music     Public  Templates
Desktop  Downloads  Pictures  snap    Videos
ruzdan@Ubuntu:~$ cd Ayan/
ruzdan@Ubuntu:~/Ayan$ ls
12116032_copy.txt
```

### 5. Create multiple directories using single command. (Directories name can be your friends' names)

Ans.

```bash
ruzdan@Ubuntu:~$ mkdir Harsh Aayush Shubham
ruzdan@Ubuntu:~$ ls
Aayush  Desktop    Downloads  Music     Public   snap       Videos
Ayan    Documents  Harsh      Pictures  Shubham  Templates
```
