# Security in Systems and Services — HRY-413 (TUC)

Eight assignments spanning applied cryptography, OS-level access control,
malware detection, network traffic analysis and web/binary exploitation, for the
Security in Systems and Services course (2024–2025). **Final grade: 8.5 / 10.**

Collaborator: [Georgios Piperakis](https://github.com/giorgosPiperakis).

> Academic coursework. Everything here was built and run against intentionally
> vulnerable targets and sample data provided by the course, for learning
> defensive and offensive fundamentals. Some assignments need extra files, linked
> from Dropbox in their own READMEs.

## Assignments

| # | Topic | Summary |
|---|-------|---------|
| 1 | **Applied cryptography (C)** | An RSA tool using GMP (key generation, encrypt/decrypt, with timing/memory benchmarks at 1024/2048/4096-bit keys) and an ECDH key-exchange tool over Curve25519 using libsodium. |
| 2 | **Access-control logging (C)** | A shared library (`LD_PRELOAD`) that intercepts `fopen`/`fwrite` to log file-access events, including denied attempts, plus an `acmonitor` utility that analyses the log for unauthorised access and modifications. |
| 3 | **Malware detection (Python)** | A signature-database builder, a multi-hash file scanner and detector, and a scan-and-quarantine tool with a directory observer for continuous monitoring. |
| 4 | **Web vulnerabilities (Flask)** | A mock web app used to study six classic vulnerability classes — two SQL injections, reflected XSS, DOM-XSS, local file inclusion and open redirect — and the fixes for each. |
| 5 | **Packet analysis (C, libpcap)** | A live/offline packet sniffer that parses IP/TCP/UDP, supports BPF-style filters, and flags TCP retransmissions by tracking flow state. |
| 6 | **Host firewall (shell)** | A domain-blocking firewall script with `config / save / load / list / reset / help` options, verified against allowed vs. blocked domains. |
| 7 | **IDS & traffic forensics (Python, Scapy)** | Crafting and analysing packets, port-scan traffic generation, Snort rules, and performance tuning over a large PCAP. |
| 8 | **Binary exploitation (C)** | A controlled stack-buffer-overflow exercise against a provided vulnerable `Greeter` program, demonstrating memory-safety failure modes. |

## Layout
```
assign_1/ … assign_8/   one folder per assignment, each with its own README/report
```

## Tech
C · Python · Flask · Scapy · libpcap · GMP · libsodium · Linux · Makefiles ·
applied cryptography · access control · malware detection · network security ·
web security · memory safety
