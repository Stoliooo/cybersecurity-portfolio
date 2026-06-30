# Lab: Search Skills

## Date
2026-06-28

## Objective
Have an understanding of the varying websites and services used to assist with both offensive and 
defensive security analysis and reconnaissance.

## Tools Used
- Shodan Simulation
- VirusTotal Simulation
- Vulnerability Database Simulation
- Linux terminal
- Linux MAN Pages
- Github Simulation (lol)

## Steps Taken
1. Searched "apache" on TryScanMe (Shodan simulation) and reviewed the first result.
2. Identified the domain associated with a given IP address from the search results.
3. Explored CVE identifiers and their naming format.
4. Submitted a file/URL to the VirusTotal simulation and reviewed the multi-engine verdict.
5. Reviewed CVSS scoring factors for a sample vulnerability.
6. Used `man nc` in the Linux terminal to explore manual page documentation.
7. Searched GitHub for relevant PoC exploit code.

## Key things learnt
1. Shodan, unlike other search engines that index websites, indexes everything and anything that is connected to the internet, and the information those devices broadcast
about themselves in real time, i.e., HTTP Headers that introduce themselves, and makes it searchable. It shows you the varying companies domains, IP ranges and oganisation names
broken down by country, organisation, and port. A pentester may find this weakness and exploit it. A defender may find this weakness and patch it.
2. CVE: Common Vulnerabilities and Exposures. It identifies and categorises known vulnerabilites in software. The CVE database is public, so hacker, pentester or defender alike may easily identify this weakness in software and its severity. The HTTP header identifies which software is running. Each confirmed vulnerability is assigned a unique identifier in the format CVE-YEAR-NUMBER, such as CVE-2025-55182. If the vulnerability is impactful enough, it may even get a moniker (eg., Heartbleed, React2Shell, and Log4Shell.)

3. Shodan filters allow you to narrow search results precisely:

| Filter | Description | Example |
|--------|-------------|---------|
| `country` | Restrict results to a specific country code | `country:IE` |
| `port` | Filter by a specific port number or range | `port:22` |
| `org` | Scope results to a named organisation or ASN identifier | `org:AS7224` |
| `hostname` | Match against a specific hostname or domain | `hostname:fakebank.thm` |

4. VirusTotal takes results from over 70 antivirus engines and website scanners into a single 
interface. You can submit a file, URL, domain, or file hash, and it returns a verdict from each engine 
on whether that item is malicious. This is useful because no single antivirus catches everything. 
Checking against 70+ engines at once gives a far more reliable picture than relying on one tool alone. 
Defenders use it to vet suspicious files or links before opening them, while pentesters may use it to 
check whether their own tools would be flagged before deploying them in an authorised test.
5. Vulnerabilities are given a score (CVSS) based on a variety of factors, such as:

- Impact - What damage can this vulnerability lead to?
- Complexity - Is the vulnerability easy to exploit or not? 
- Availability - How likely is it that someone can exploit this?
6. MAN pages, short for "manual pages", are Linux's built-in documentation system. Every command-line tool on Linux typically has one. Instead of memorizing flags like gobuster -u -w, MAN pages are how you start being able to look things up. Also, that nc means netcat.
7.  Researchers often publish proof-of-concept (PoC) code, exploitation tools, and detailed technical reports here on Github, which is usually faster than official channels. This makes GitHub valuable recon during a pentest - searching for leaked credentials, exposed API keys, or PoC exploits relevant to a target's tech stack.

## Notes
- `nc` = netcat, a networking utility for reading/writing across network connections.
- Man pages exist for most CLI tools; if a tool lacks one, try `--help` instead.
- TryScanMe and the VirusTotal simulation mimic real-world tools without needing live accounts.

## Commands Used
```bash
user@thm$ man nc
