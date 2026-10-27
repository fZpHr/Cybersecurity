# Cybersecurity

42 student working on binary exploitation, reverse engineering and security tooling.
This repository indexes my security projects and the skills behind them.

## Tooling

**[Kintsugi](https://github.com/fZpHr/Kintsugi)**: self-hosted multi-decompiler
explorer, forked from Decompiler Explorer (dogbolt.org). Runs 9 decompilers
(Ghidra, angr, RetDec, Reko, rev.ng…) on a binary, then uses an LLM to merge their
outputs into a single listing, keeping each function's source visible, before a
second pass names and annotates it. Django + Docker Compose, pluggable LLM backends
(Gemini, Claude, OpenAI-compatible).

**[CTF: La Quete du Stagiaire](https://github.com/fZpHr/CTF)**: a multi-stage CTF
I designed and deployed. Web recon, SSH access, privilege escalation (sudoedit CVE),
then sniffing cleartext traffic. Vulnerable-by-design services behind nginx,
orchestrated with Docker Compose. Categories: web, privilege escalation, forensics, network.

## Binary exploitation & reverse (42)

- **[Override](https://github.com/fZpHr/override_42)**: buffer overflow, ret2libc,
  format string, GOT overwrite, shellcode, out-of-bounds write, ptrace anti-debug; x86 32/64-bit.
- **[Rainfall](https://github.com/fZpHr/rainfall_42)**: stack overflows, format strings,
  32-bit exploitation, privilege-escalation chain.
- **[SnowCrash](https://github.com/fZpHr/snow-crash_42)**: Linux wargame with setuid, cron,
  scripting, and traffic/forensics challenges.
- **[libasm](https://github.com/fZpHr/libasm_42)**: C standard-library functions
  reimplemented in x86-64 assembly; the low-level fluency behind the reverse work.

## Web exploitation (42)

- **[Darkly](https://github.com/fZpHr/darkly_42)**: found and exploited the flaws of a
  deliberately vulnerable site: SQL injection, path traversal, request tampering / IDOR,
  brute force, weak cookie hashing, and open redirect.

## Cybersecurity Piscine (42)

Fundamentals across six projects ([repo](https://github.com/fZpHr/Piscine_Cybersecurity_42)):

| Project | Area | Summary |
|---|---|---|
| Arachnida | Web | web scraper + image EXIF metadata extraction |
| ft_otp | Crypto | TOTP generator (RFC 4226, HMAC) |
| ft_onion | Web / infra | Tor hidden service behind nginx |
| Reverse me | Reverse | binary analysis |
| Stockholm | Malware | educational ransomware (RSA / AES) |
| Inquisitor | Network | ARP spoofing / traffic analysis (MITM) |

## Skills

- **Binary exploitation:** buffer overflow, ret2libc, format string, GOT/PLT overwrite,
  shellcoding, out-of-bounds read/write; familiarity with ASLR, NX, stack canaries, ptrace anti-debug.
- **Reverse engineering:** Ghidra, gdb/gef, objdump/readelf, decompiler-output analysis;
  built RE tooling (Kintsugi).
- **Web:** recon & enumeration (gobuster, nmap), web-app exploitation (SQL injection,
  IDOR, path traversal), scraping, Tor hidden services, nginx.
- **Network:** ARP spoofing / MITM, packet capture & analysis (pcap).
- **Crypto:** TOTP/HOTP (HMAC), RSA / AES in practice.
- **Malware:** ransomware internals (encryption, file traversal), educational.
- **Systems:** Linux privilege escalation, setuid, known-CVE exploitation (Exploit-DB).
- **Dev / infra:** Python (Django), C, Bash, x86 assembly, Docker Compose.
