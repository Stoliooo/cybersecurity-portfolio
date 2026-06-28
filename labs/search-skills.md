# Lab: Search Skills

## Date
2026-06-28

## Objective
Have an understanding of the varying websites and services used to assist with both offensive and 
defensive security analysis and reconnaissance.

## Tools Used
- Shodan
## Key things learnt
1. Shodan, unlike other search engines that index websites, indexes everything and anything that is connected to the internet, and the information those devices broadcast
about themselves in real time, i.e., HTTP Headers that introduce themselves, and makes it searchable. It shows you the varying companies domains, IP ranges and oganisation names
broken down by country, organisation, and port. A pentester may find this weakness and exploit it. A defender may find this weakness and patch it.
2. CVE: Common Vulnerabilities and Exposures. It identifies and categorises known vulnerabilites in software. The CVE database is public, so hacker, pentester or defender alike may 
easily identify this weakness in software and its severity. The HTTP header identifies which software is running.
The issue is you put the table inside a code block (the triple backticks). That makes markdown render it as plain text instead of an actual table.
```markdown
3. Shodan filters allow you to narrow search results precisely:

| Filter | Description | Example |
|--------|-------------|---------|
| `country` | Restrict results to a specific country code | `country:IE` |
| `port` | Filter by a specific port number or range | `port:22` |
| `org` | Scope results to a named organisation or ASN identifier | `org:AS7224` |
| `hostname` | Match against a specific hostname or domain | `hostname:fakebank.thm` |
```
4.
