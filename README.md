# firebird-recovery-tool
Read-only Firebird recovery tool. Repair corrupted Firebird database files and damaged backup files, supports Firebird 1.0–5.0.
# Firebird Recovery Tool

A read-only Firebird recovery utility for corrupted database files and damaged backup files.

## Overview

Firebird Recovery Tool performs offline, read-only analysis on Firebird database files and backup files. It parses corrupted database structures directly, extracts usable table data from broken files, and salvages records from damaged backups without writing any changes to your source evidence.

All scanning operations run in **read-only mode** — your original database files and backup files remain untouched.

## Supported Versions

- Firebird 1.0
- Firebird 1.5
- Firebird 2.0
- Firebird 2.1
- Firebird 2.5
- Firebird 3.0
- Firebird 4.0
- Firebird 5.0

## Core Capabilities

- Repair and recover data from corrupted Firebird database files (`.fdb`, `.ib`)
- Recover data from damaged Firebird backup files (`.fbk`, `.gbak`)
- Extract table data from broken, unmountable or inconsistent database files
- Preview recoverable table data before export
- **100% read-only scan**: source files will never be modified

## Use Cases

- Firebird database file corruption
- Damaged or broken backup files
- Database file cannot be attached or opened
- Data rescue from corrupted FDB/IB files
- Recovery from damaged GBAK/FBK backup files

## How It Works

1. The tool scans the corrupted Firebird database file or backup file in read-only mode.
2. It parses internal database page structures directly.
3. Recoverable tables and records are identified and extracted.
4. Recoverable data is displayed in a preview view.
5. Verified data can be exported after preview.

## Important Notice

This is an offline forensic analysis tool.

We do **not** write or modify the original database files or backup files during scanning. Always work on copies of your source files for evidence safety.

## Download

Get the latest Windows binary release on GitHub Releases.

> Pre-built Windows x64 zip package, contains the read-only Firebird recovery client.


## Antivirus Note

> ⚠️ The Windows binary is protected with VMProtect for anti-tampering. Some antivirus software may incorrectly flag it as malware (false positive). This tool works in fully read-only mode and will not modify your database source files.

## Contact

For technical feedback, bug reports or feature requests, please open a GitHub issue.
