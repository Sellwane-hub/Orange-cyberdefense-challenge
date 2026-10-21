# Orange Cyberdefense / SensePost Academy Staged Web Application Challenge

A penetration test report documenting a nine level staged web-application
security challenge hosted by Orange Cyberdefense (SensePost Academy).

Target:challenge.orangecyberdefense.academy
Date:24 September 2026
Result:Levels 07 completed in full; Level 8 reached and investigated
Standards:CVSS v3.1 scoring, OWASP Top 10 (2021), PTES methodology

## Overview

The challenge presented a series of web-application levels, each protected by a
different client-side security mechanism. Each level was approached with a
consistent process: reconnaissance and enumeration, analysis, a single
hypothesis, exploitation, and evidence capture before moving on.

## Techniques demonstrated

- DNS reconnaissance and TXTrecord information disclosure
- Hardcoded credentials recovered from page source
- Base64 and multiencoding secret recovery
- Reversible client-side cryptography (crypto-js with a Sudoku-derived key)
- Hidden route concealed in a QR code among decoy content
- Command-line inspection to bypass browser-side restrictions

## Key finding

Security decisions and secrets were enforced in the browser rather than on the
server. Passwords, keys, and routes were all recoverable by any user willing to
inspect the client-side code. The five recurring weakness themes and their
remediation are detailed in the report.

## Report

See the full report: Orange cyberdefense report.pdf

## Tools

nslookup, dig, curl, base64, binwalk, exiftool, zbarimg, nmap, Burp Suite — Kali Linux

Author: Sellwane Suzan Matsheka · Computer Systems Engineering graduate, Tshwane University of Technology
