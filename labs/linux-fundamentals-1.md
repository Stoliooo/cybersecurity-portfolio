# Lab: Linux Fundamentals I

## Date
2026-07-01

## Objective
Run commands on an interactive Linux machine, learn some essential commands used to interact with the file system and understand how users work in groups 
utilizing Linux.

## Tools Used
- Ubuntu Linux Machine
- 

## Steps Taken
1. Booted up the Ubuntu Linux Machine
2. 

## Key Things Learnt
1. "Linux" is not a single operating system — it is a general term for a family of UNIX-based 
operating systems. Because UNIX is open source, many variants (called distributions or "distros") 
exist, each tailored for specific use cases. For example, Ubuntu for general use, Kali Linux for 
penetration testing, and Ubuntu Server for hosting web servers.
2. Even though cat was made for the sole purpose of joining two or more directories together, 
it's most popular use is the viewing of a file in a directory. This is refered to as the UUOC, or 
the Useless Use of cat.
3. One can use cat to output the contents of a file within directories without having to navigate
to it by using cat and the name of the directory. I.e. cat /home/ubuntu/Documents/todo.txt
4. In instances, cat can be used to retrieve usernames, passwords(💀), flags or configuration settings are stored within files where 
"cat" can be used to retrieve these.
5. If using find and the name of the file is not known to you, you may use a wildcard (*) to search for anything that is that file type.

## Notes
- echo - Output any text that we provide (If echoing a single word, no quotes are needed. However quotes will be needed if it is a statement)
- whoami - Find out what user we're currently logged in as
- ls - Listing (Shows all directories/folders in the system. Using ls with one of those directories/folders would outline the contents of said directory/folder)
- cd - Change Directory (current/working Directory)
- cat - Concatenate (combine/join)
- pwd - Print Working Directory
- find - Automate Search for Files
- grep - Find Specific Values (like say, a specific IP, and the things a specific IP has visited based on access log entries)
- -R - Recursive (used with grep)

## Commands Used
