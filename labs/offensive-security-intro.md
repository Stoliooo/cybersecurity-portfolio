# Lab: Introduction to Offensive Security

## Date
2026-01-22

## Objective
Understand the basic concepts of offensive security and how attackers
approach exploiting systems.

## Tools Used
- Linux terminal
- TryHackMe offensive security lab environment
- Gobuster

## Steps Taken
1. Learned what offensive security is.
2. Explored how vulnerabilities are identified and exploited.
3. Interacted with a vulnerable target system in a controlled lab environment.
4. Performed directory enumeration on the target web application using Gobuster.
5. Used a common wordlist to identify hidden directories that are not directly linked on the site.

## Key Things Learned
1. A command line application named "Gobuster", used in terminals, which may be used to brute force a website and find hidden directories and pages

## Notes
- Remember that directory enumeration should always be done ethically.
- `gobuster` flags: -u for target URL, -w for wordlist, dir mode for directories.
- In future labs, try combining Gobuster with Nmap results for better recon.

## In the command below, -u is used to state the website we're scanning, -w takes a list of words to iterate through to find hidden pages.


## Commands Used
```bash
gobuster -u http://fakebank.thm -w wordlist.txt dir


   
