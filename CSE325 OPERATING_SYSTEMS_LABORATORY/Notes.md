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

1. Explore the file system of a Windows system and a Linux system, and write prime differences.

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
